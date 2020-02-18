# OLED Remotes \[Under Development\] \[Please leave suggestions\]

### Replies: 295 Views: 12851

## \#1 Posted by: Sander Posted at: 2017-04-30T02:29:01.242Z Reads: 854

```
_Before reading:_
**Please do not feel that you are interrupting the flow of ideas or anyone else who is reading this thread and has an idea. Though few people are discussing the remote, being developed on this thread, I have continued to reply publicly so that this controller can be made as good as it possibly can be - I am sure that other people will input valuable ideas based on their experiences and will value seeing the thought process behind decisions. Please reply with ideas of things you would like added to the code and changes to the design to make it look less bulky!**
- @Print3r 


Hello! I have created the WINNING Remote shell from scratch with OLED place in Fusion 360.
In the OLED Remote.zip you have two options, A tight fit one, or a more loose one for the OLED.
When you install the OLED **do not push it hard** otherwise it will break like my 6 other oleds...

If you 3D print it post it below  :slight_smile:
Because I cant 3D print it right, I broke a part for the stepper motor. 

_You are allowed to modify and sell it but you need to give me credits for 3D Modeling it and if selling ask the WINNING Company for permission._ 
**License:** https://creativecommons.org/licenses/by/4.0/

**This is not a 100% Accurate Copy of it.** 

<img src="/uploads/db1493/original/3X/4/2/42b3ed27232814929c3957fd1240599c06093066.png" width="690" height="361">

<img src="/uploads/db1493/original/3X/7/c/7c527451fddcd863a4ef66d6c82c0535380fba5f.png" width="690" height="361">


<img src="/uploads/db1493/original/3X/2/2/22082f63b20bd198b91a214eae8d0f457c1f5d6b.png" width="690" height="361">

<img src="/uploads/db1493/original/3X/5/6/56b13019eaf50d3b7ceb53ec4e60b4f2931c1654.png" width="445" height="500">


----------

I would love to show a video of my remote with the oled, but I broke it by pressing it to hard.

<img src="/uploads/db1493/original/3X/d/7/d794cbe86cda63d8c8d0b8ad8ce868821626fc8f.jpg" width="374" height="500">


----------

I will create a PCB that are Arduino compatible and compatible to this shell. I am waiting for my custom pcb that runs on ATmega32U4. If I succeed I will move forward and create one for this shell. 

----------

My PCB looks like this:
<img src="/uploads/db1493/original/3X/0/c/0c8f8448db1845a7153a8f5efffa01e5a73c2c54.png" width="690" height="447">


----------

Download with room for OLED:

https://www.dropbox.com/s/bb609dr9dewffhm/OLED%20Remote.zip?dl=0

Download without room for OLED:

https://www.dropbox.com/s/xtbr74zeir4y0wj/Remote.zip?dl=0
```

---
## \#2 Posted by: wmj259 Posted at: 2017-04-30T03:05:37.834Z Reads: 727

```
Is this like a better version of the winning remote or a copy of it?
```

---
## \#3 Posted by: Sander Posted at: 2017-04-30T03:08:00.682Z Reads: 731

```
[quote="wmj259, post:2, topic:22055, full:true"]
Is this like a better version of the winning remote or a copy of it?
[/quote]

Its a copy ready for 3d printing.
I did this because I really like how it looks and how small it is. 
Inside it I have my own electronics not the unreliable winnings remote.

Technically it's a better version because its reliable and has a display that shows the current ampere, voltage, speed with a menu that you can change the light colors, speed, acceleration, where to turn when you have enabled the GPS Destination etc.
```

---
## \#4 Posted by: lox897 Posted at: 2017-04-30T03:35:59.624Z Reads: 676

```
Really nice work with this! Love your PCB skills! Do you know what part the winning uses for the thumb wheel? Joysticks are quite wide so I am looking for a better alternative
```

---
## \#5 Posted by: Print3r Posted at: 2017-04-30T09:42:17.029Z Reads: 645

```
I do not know what part they use but found a simple pot on ebay (http://www.ebay.co.uk/itm/2-PCS-Piher-Potentiometer-PT15-Rotor-16mm-WHITE-RED-/220651549590?hash=item335fdb7396). If a thumbwheel was then 3D printed (with two holes near the edge 180o apart from each other), then put a spring between casing and holes on thumbwheel for both sides of the thumbwheel and two part epoxy the thumbwheel to the rotating part on the potentiometer. Then you have a thumbwheel!

I assume you are using RollingGecko's code from Github? If not, what does yours do differently?
```

---
## \#6 Posted by: Sander Posted at: 2017-04-30T10:10:24.783Z Reads: 635

```
[quote="Print3r, post:5, topic:22055"]
I assume you are using RollingGecko's code from Github? If not, what does yours do differently?
[/quote]

I do not use RollingGecko. I made my own hardware. The difference is I can change values with my controller. Like turning on/off lights, change the light color, the max speed, max ampere and acceleration.

Here is an example, its a old video much has changed.:
https://www.youtube.com/watch?v=FX_vr-hvWRk
```

---
## \#7 Posted by: Sander Posted at: 2017-04-30T10:12:54.789Z Reads: 592

```
I found a spring loaded thumb wheel:
http://www.elobau.com/en/operator-controls/thumbwheels/thumbwheel-151dt01
```

---
## \#8 Posted by: Print3r Posted at: 2017-04-30T10:17:32.760Z Reads: 568

```
Will you open source your software at the end so others can use - it looks amazing? I am thinking of doing this next year but maybe also integrating some gps navigation using Google maps API, bluetooth to transfer data and gps to know when the next direction should be displayed. Having something like this: https://snazzymaps.com/style/79/black-and-white on an lcd display would also be quite cool.

The problem I have with that thumbwheel is that it looks like it returns to very back when released - I would prefer if it went to the middle or to 1/3 from back (if you see what I mean).
```

---
## \#9 Posted by: Sander Posted at: 2017-04-30T10:26:51.338Z Reads: 586

```
Yes I have thought about that. Before I had bluetooth connected and I could change values and controll the speed with my iphone. I think about having an ESP8266 that host an access point to show where you have driven and the good thing with having an ESP8266 I can have wireless updating. I will have a gps module that gets logged on a sd card. The ESP reads from the sd card and writes it to the client. The gps gives me the local time too so I will  have a bar in the middle of the oled in the controller displaying the current time.

But I think having two system that uses wire to communcate, because I dont want the reciever to UART to get slowed down etc.

 [quote="Print3r, post:8, topic:22055"]
The problem I have with that thumbwheel is that it looks like it returns to very back when released - I would prefer if it went to the middle or to 1/3 from back (if you see what I mean).
[/quote]

Ohh I forgot that, I get what you are saying ;)¨

Well the bad thing about having that map on the oled is that I need to be connected to the internet. But its doable I think. But it will be hard to see on the oled. I will give it a try in the future?

Its an easy fix to get it go back in the middle, I will 3D design it now.
<img src="/uploads/db1493/original/3X/1/f/1f6a0c2de9dbdaa86c509a19a8510076c3528a09.png" width="450" height="450">
```

---
## \#10 Posted by: Print3r Posted at: 2017-04-30T10:37:28.447Z Reads: 530

```
Seems like you have an idea how to do it! I am going to have to research how the ESP8266 works and how to get the app to copy some text from a webpage to understand your code I think! Please post pictures if you get this working. I will upload in 30 minutes a stl of the thumbwheel I was talking about to thingiverse and will post link here.
```

---
## \#11 Posted by: Sander Posted at: 2017-04-30T11:03:56.846Z Reads: 507

```
Cool! If you want ESP8266 to get things from webpage you can use an API called ThingSpeak and use HTML XPATH. On the ESP you use HTTP Request.
```

---
## \#12 Posted by: Print3r Posted at: 2017-04-30T11:24:16.938Z Reads: 505

```
Thanks for the explanation, my main idea is the gps directions not the map (map was just cool addition but really useless because so small)! I don't have the time to work on this until June but I assume it is going to involve setting up a website, inputting start point and destination, then fetching the directions from Google and weeding out all the unnecessary stuff. Then this script has to be transferred over ESP8266 wifi to the arduino(s) that have bitmaps for the Turn left, turn right instructions and a gps. The screen will then display metres to where you need to turn, which way you need to turn, then a line, then speed in top right, then km/miles left (based on gps and watt hours). This code is beyond me for the moment, so good luck if you are going to try it - you seem to know a lot more! By the way, I couldn't find the use of Thingspeak in this application (perhaps it is my insufficient knowledge of coding) I did understand Xpath though!
```

---
## \#13 Posted by: Print3r Posted at: 2017-04-30T11:49:04.071Z Reads: 493

```
5 minute thumbwheel creation (will be updated in June when I design my controller): 
http://www.thingiverse.com/thing:2284623
```

---
## \#14 Posted by: Sander Posted at: 2017-04-30T11:49:56.978Z Reads: 496

```
Very cool idea! I can join you. I have already created a meter counter with the gps. Not 100% accurate yet.. Here is the code I have made:

https://pastebin.com/GEQD1aau
```

---
## \#15 Posted by: Sander Posted at: 2017-04-30T15:48:23.011Z Reads: 497

```
And for the gps you can also use an accelerometer inside the board that shows the way. The arrow will move dynamic of the way the board is pointed.
```

---
## \#16 Posted by: Sander Posted at: 2017-04-30T16:48:31.473Z Reads: 507

```
Well here is my updated thumbstick:
https://www.youtube.com/watch?v=0biJaJocvLk&feature=youtu.be
```

---
## \#17 Posted by: Print3r Posted at: 2017-04-30T16:52:41.301Z Reads: 509

```
If I understand your reply as something like this (https://www.kickstarter.com/projects/1411369083/beeline-smart-navigation-for-bicycles-made-simple), I think that a gps with turn signals would better. A dynamic rotating arrow based on the direction of the board that showed you which exit on every turn to take would be cool, but hard to implement with the Google API. It also would be harder to interpret on some roundabouts where the exits are close together. To make connections clear, I have started a list below (connections I am unsure about in italics)

Nano connections possible: SPI, Serial, I2C and 

Receiver on board: Tx, Rx, 5v 0V connected to VESC, SPI connections to nRF24L01+,
Transmitter arduino nano 1: _Serial connection to other nano_, SPI connections to nRF24L01+, I2C screen
Transmitter arduino nano 2: _Serial connection to other nano , GPS connection, ESP8266 wifi connection to phone (app/ webpage will produce some data that needs to be transferred across using wifi), sd card connections_

I use solidworks but am trying out Fusion 360 because it renders fast and beautiful! :) I think the thumbstick should have a knob to indicate where it is - the bobbles will give grip but won't allow you to know where it is (if you see what I mean). It certainly looks more professional than mine, but don't know where the spring connections go - is it a 'copy' of the linked one or an improved version that returns to half-way/ 1/3 of the way up.

Didn't mean for this to be so long!
```

---
## \#18 Posted by: Print3r Posted at: 2017-04-30T16:59:34.086Z Reads: 489

```
On watching a second time I think I understand (see image)<img src="/uploads/db1493/original/3X/e/1/e1f8a86331130613b2ae47cae47c5403e36eb75f.png" width="629" height="500">

Or is the long bit of the spring stuck between the top things on the rotating part of the thumbstick?
```

---
## \#19 Posted by: Sander Posted at: 2017-04-30T17:03:50.220Z Reads: 493

```
[quote="Print3r, post:17, topic:22055"]
I think the thumbstick should have a knob to indicate where it is
[/quote]

Yeah I was going to add it but I forgot it.

[quote="Print3r, post:17, topic:22055"]
don't know where the spring connections go
[/quote]

Almost, but I will use one in the middle.
The spring is in the middle of the static overhang, with the two cylinders(More like a metal thread, then a spring).
<img src="/uploads/db1493/original/3X/b/d/bdb681c5d1afd09bbd2cbcf2f18185ab09a8797f.png" width="690" height="388">

And the gps bike thing is just like what I meant! I didnt fully understand what you meant with the connections, on second thought I think what you mean. 

For the GPS, we could have a setting with "Auto Turn Signal". So when you are 5 meters before a turn to the right it will blink for you automatic.
```

---
## \#20 Posted by: Print3r Posted at: 2017-04-30T17:19:24.315Z Reads: 463

```
Got it now for the thumbstick! Do you agree about the arrow or would you prefer it - I suppose if you know which way you should head that is much simpler, uses up less memory and has less to go wrong! Also, everyone should be able to follow an arrow and easier to learn about a place if you do not blindly follow instructions but work it out! I was just thinking that bluetooth is compatible with everything, so connect bluetooth module to serial of transmitter nano 2 and then send a string (latitude and longitude) to the bluetooth module of transmitter nano 2. Problem is that currently the serial port of the transmitter arduino nano 2 is connected to the other transmitter nano!
```

---
## \#21 Posted by: Sander Posted at: 2017-04-30T17:24:43.881Z Reads: 408

```
[quote="Print3r, post:20, topic:22055"]
Problem is that currently the serial port of the transmitter arduino nano 2 is connected to the other transmitter nano!
[/quote]

No problem with the serial port, we can just use the SoftwareSerial for more Serial Ports.
```

---
## \#22 Posted by: Print3r Posted at: 2017-04-30T17:25:56.340Z Reads: 394

```
Cool! Need to think about screen size soon.
```

---
## \#23 Posted by: Sander Posted at: 2017-04-30T17:29:55.603Z Reads: 393

```
0.96" Screen is plenty if its just going to be an arrow.
```

---
## \#24 Posted by: Print3r Posted at: 2017-04-30T17:31:25.821Z Reads: 398

```
Ideally I would also like speed and miles left (based on battery usage). Having your settings option would be cool but that seemed v.complicated to do!
```

---
## \#25 Posted by: Print3r Posted at: 2017-04-30T17:43:31.322Z Reads: 395

```
1.3" seems to be the biggest possible without getting too expensive. So will make proof of concept controller with that in mind. (https://www.adafruit.com/product/938) - probably won't buy from adafruit though.
```

---
## \#26 Posted by: Sander Posted at: 2017-04-30T17:56:32.642Z Reads: 389

```
I have a much better idea with the tracking system.
In Xcode I can make an map application, that connects via bluetooth. So you know the apple map that shows arrow and when to turn left. I have the same thing and send that data to the bluetooth and visualize it with the oled. Much easier and faster. But I have no idea of making that into an android application.
```

---
## \#27 Posted by: Print3r Posted at: 2017-04-30T17:59:30.184Z Reads: 403

```
I have an iphone so android can be added if others are interested and know how to do it! Starting to like Fusion 360 more and more - not any random errors so far, just everything is in a different place to solidworks!
```

---
## \#28 Posted by: Sander Posted at: 2017-04-30T18:00:25.486Z Reads: 416

```
And the joint tool is amazing too.
```

---
## \#29 Posted by: Print3r Posted at: 2017-04-30T19:01:41.872Z Reads: 444

```
Design 1 link is here (it is a first draft - only the measurements of the screen are right):
http://a360.co/2qilVYi
Render with info below:
<img src="/uploads/db1493/original/3X/d/e/deca2bae5efd328afb777d39b270fd0c79d519bc.png" width="690" height="389"> 
Please change dimensions/ everything you want/ start afresh but I will have little time to do any more design/ coding work during the week. My controller design seems very clunky so I will have to find ways to make it look cooler - maybe add some useless fins and some bevels in places. Handles will also need finger dents in them. I just understood the timeline feature towards the end of editing - I could not find the usual 'edit feature' button from solidworks so there are some additional extrusions!

2.4ghz module with antenna and amplifier http://www.ebay.co.uk/itm/NRF24L01-PA-LNA-SMA-Antenna-Wireless-Transceiver-communication-module-2-4G-1100m-/201701854993
I2C 1.3" screen http://www.ebay.co.uk/itm/1-3-inch-IIC-I2C-128X64-Blue-OLED-LCD-LED-Display-Module-for-Arduino-Hot-/252779086984
Cheap arduino nanos: https://www.aliexpress.com/item/Freeshipping-10pcs-lot-Nano-3-0-controller-compatible-for-arduino-nano-CH340-USB-driver-NO-CABLE/32326740961.html
Gps: https://www.ebay.co.uk/p/?iid=272508603552&&&adgroupid=43333907642
Lipo: https://www.banggood.com/Eachine-3_7V-500mah-25C-Lipo-Battery-for-Hubsan-H107-H107L-H107C-H107D-p-993951.html
```

---
## \#30 Posted by: Sander Posted at: 2017-04-30T19:06:18.749Z Reads: 396

```
looks cool!
```

---
## \#31 Posted by: Sander Posted at: 2017-04-30T20:17:10.731Z Reads: 386

```
I got a VERY good idea!
You know you need to use 4G to use the map to get location. If I use the GPS Module and send current location to my phone via bluetooth you won't need to use 4G nor Internet. And selecting places does not need 4G either, only searching. But to load the map you need 4g...
```

---
## \#32 Posted by: Print3r Posted at: 2017-04-30T20:49:46.193Z Reads: 374

```
You don't need 4g to get location (your phone has a gps chip inside) - on some gps apps you can download the map so it is offline then you don't have to pay data charges (but you don't know traffic like with waze). A user should only need to put in his destination at the start of a ride and should have wifi then - starbucks/ home wifi/ work wifi. If not, one internet search uses hardly any data, but good idea. Actually, the user could be given the choice to get the longitude and latitude from one of the apps where you can download the map offline. Then copy and paste that into a super simple, 'upload this string to the arduino nano controller' app.
```

---
## \#33 Posted by: Sander Posted at: 2017-04-30T21:02:56.357Z Reads: 362

```
But I have a hard time finding and creating Turn by Turn navigation....
```

---
## \#34 Posted by: Sander Posted at: 2017-04-30T23:43:13.537Z Reads: 422

```
Okey progress is being made! I have now created an application with the MapKit in Xcode, now it tells me currently the steps. I will try to figure out with the turn to left in 50 meters soon. Right now its like this:

> Proceed to Arne Garborgs veg
> Use the roundabout to make a U-turn
> At the roundabout, take the second exit onto Jernbanegata
> At the roundabout, take the first exit onto Meierigata
> Arrive at the destination

I got an idea how to make it say turn left in 50 meters.
If I take the distance and check if text contains left, then I can format it in to "Turn Left in 50m"

for step:MKRouteStep in steps{
print("Distance: \(step.distance)")
print("Instruction: \(step.instructions)")
}

This is how it looks like(I can change road types, like bike path, walking etc, so it chooses your preference):
<img src="/uploads/db1493/original/3X/9/1/91c9dad8416c9a3593abf5f9cd75a6f8c4fc7d40.png" width="284" height="500">

This is good I tested it on another road with no roundabout, only straight roads.
> *Distance(In): 0.0m 
> *Instruction: Proceed to Keep
> *Distance(In): 405.0m 
> *Instruction: Turn right onto IngThis
> *Distance(In): 123.0m 
> *Instruction: Turn left onto Secret
> *Distance(In): 90.0m 
> *Instruction: Turn right onto ForMyOwn
> *Distance(In): 52.0m 
> *Instruction: Turn left onto Privacy
> *Distance(In): 5.0m 
> *Instruction: Arrive at the destination

I can format it if I get a "Turn left onto Anon". And let it show a left arrow with the meter below of it.

And the good thing with it going thru all the steps. I can upload the destination to the sd card, it will give name on the cordinates etc. But if you take a wrong way it will not tell you tho..
```

---
## \#35 Posted by: Print3r Posted at: 2017-05-01T07:13:33.138Z Reads: 377

```
a) it looks amazing
b) The problem of 'if user goes off-route' is one I have been thinking about'. 
      i)If the location of each junction is given, could there be a small rotating arrow in the top of the screen that points to the next junction (based on the way the accelerometer is pointed) - that way if you go off track you can just follow that arrow to rejoin your route. 
      ii)GPS Navigation by Scout was the offline navigation app I was thinking of, but their api seems to be getting updated and by the sounds of it, you have to pay so rerouting offline is not possible unless you can do it offline with google/ apple maps api. My idea with the offline reroute is that when a reroute is sensed (I assume that if in offline mode you could get the app to calculate a reroute every 30 seconds) the phone sends a bluetooth packet so the controller shows 'Reroute being calculated' and then sending the new route. 
     iii) Find all the junctions around the route at the start and say u-turn when the user gets there.

Option i) seems easiest then iii) then ii). What do you think?
```

---
## \#36 Posted by: Sander Posted at: 2017-05-01T07:23:07.656Z Reads: 343

```
Well if your phone is connected to internett/4G, and you drive wrong it will tell you on the remote.
```

---
## \#37 Posted by: Print3r Posted at: 2017-05-01T07:23:50.667Z Reads: 341

```
That is fine then! Does it include speed limits ;)?
```

---
## \#38 Posted by: Sander Posted at: 2017-05-01T07:27:22.079Z Reads: 361

```
It is not that bad using 4G for it, hmm speed limits dont think so. Well the eyes should be on the road so you should see a sign but it would be cool to have the speed limit. 

I am soon finished with the software. Right now the GPS sends the Latitude and Longitude via bluetooth to my phone. On my phone it chooses that as a source location(Like current position). The map updates dynamic, you choose a location to go to, it auto routes for you on the iphone. I have managed to send data back with the bluetooth with a string that contains: "AR,11.0" that gets encoded to "Turn right in 11 meters." Or just a symbol with the meters below it. But the update rate is 1-2 seconds.
```

---
## \#39 Posted by: Print3r Posted at: 2017-05-01T07:39:05.602Z Reads: 351

```
Great! The speed limit was a joke - my board I am planning shouldn't be able to get to more than 21mph (first board so playing it safe) but will be a 7s6p - 340Wh of power! The encoding looks simple but understandable. I think the update rate (assumed from phone to remote) is good - electric skateboarding is not rally driving so the instructions don't have to be given super fast, but too slow and you could be convinced you are going the right way when you aren't and forget to check the screen again.
```

---
## \#40 Posted by: Sander Posted at: 2017-05-01T07:43:51.128Z Reads: 361

```
I thought about that too. The updating rate isnt bad and when you shall turn you always slow down, or mostly because of the road rules. And it updates 1 - 1.5 seconds. It's an easy fix. All I need to do is changing the baudrate for the bluetooth. Right now its on 9600 and creates a delay when you send a long float value to it, like the cordinates that contains over 7 numbers 00.000000. But it works!

The arrow to pointing to correct place should be useful, because sometimes the gps jumps a few meters and then it will show you the wrong turn, but if you use the compass you can sync it with the phone, and get the right directions.

My first board was also 21mph plenty of speed there!
```

---
## \#41 Posted by: Print3r Posted at: 2017-05-01T08:08:29.902Z Reads: 282

```
I am wondering if the phone gps should be used (rather than a separate one in the remote) as the one in the phone is probably more accurate. Don't know if there is enough data for current longitude and latitude to also be sent - as you said, each one contains over 7 numbers!
```

---
## \#42 Posted by: Sander Posted at: 2017-05-01T08:19:18.396Z Reads: 302

```
The sending is not a problem. But I think I will leave two options. 
1. Using Phone = 4G, RIP Battery
2. Using GPS in board with downloaded map on phone with no internet/4g = Healthy battery.

I can make it in two options though. But I will choose the second one for now. I can even connect a GSM module to the board so if it gets stolen you can track it everywhere in the world.
```

---
## \#43 Posted by: Sander Posted at: 2017-05-01T08:52:57.358Z Reads: 306

```
I think I have changed my mind. I want everything going on the phone. The phone will send the data and when to turn. Much more simple and faster.
```

---
## \#44 Posted by: Print3r Posted at: 2017-05-01T09:18:42.782Z Reads: 324

```
Nearly finished replicating exactly a 2.4ghz antenna - I think the back of my first design looked to big and clunky, so seeing if maybe I can get the antenna to come up the middle of the back of the screen and have the back of the screen look like it is molded around the antenna. Also redoing the remote at the same time - started the grip, have made indents for fingers and a hole for the thumb stick (unsure of its dimension though). I like the idea of the phone doing the brunt of the work - my board will have a 5000mah fast-charge battery pack on it so I can charge my remote and maybe my phone as well when not riding!
```

---
## \#45 Posted by: Print3r Posted at: 2017-05-01T09:36:11.675Z Reads: 348

```
2.4ghz antenna (all measurements from a datasheet): 
<img src="/uploads/db1493/original/3X/4/d/4d0769ea0fd5d83a6cc4e7da18d18b99bd7a3a81.PNG" width="389" height="500">
```

---
## \#46 Posted by: Print3r Posted at: 2017-05-01T12:31:23.506Z Reads: 359

```
OLED remote v2 (see pictures below). 
2.4ghz antenna    http://a360.co/2pxvXCb
OLED controller v2  http://a360.co/2p0tn6v
Round holes at the front are for leds/ arrays of leds. Switches can be put on the sides or below the screen. The thumbstick goes in the slot on the handle. The grip has got finger dents in them, I put the antenna where it is, so that the signal from the transmitter only has to go through plastic not the palm/ fingers of a hand which will weaken it.

<img src="/uploads/db1493/original/3X/1/6/16ba1d5a17360a55b4bcdd56e242cb87f036d634.PNG" width="690" height="387"><img src="/uploads/db1493/original/3X/8/a/8a74d998609e2e1aa1e025e92853ba02ae2aa963.png" width="690" height="387"><img src="/uploads/db1493/original/3X/e/0/e0d080751a8ae1f6beefbb75764ae8bb4340efc3.png" width="690" height="387"><img src="/uploads/db1493/original/3X/d/1/d1ec876bd570bb1882eedeaaea5567e76044fd78.png" width="690" height="387">:
```

---
## \#47 Posted by: Sander Posted at: 2017-05-01T17:42:22.651Z Reads: 335

```
You know you can use a smd antenna component?
<img src="/uploads/db1493/original/3X/0/8/08269a2dae69b848bb525794399d25f7fb54b969.jpg" width="200" height="133">
But I dont know if it will work. Its rated on 2.4ghz.

The controller looks very cool! Looks like someone is showing the middle finger in the front :smile:
```

---
## \#48 Posted by: Print3r Posted at: 2017-05-01T17:48:20.600Z Reads: 333

```
I know there are SMD antennas, but I do not want a signal drop - hence the massive antenna rated for 1000m. On an e-board, I rate safety highly - no signal drops is the aim. I was hoping it would appear more like a face but now you raise the middle finger image ... it does look like a middle finger (will have to change that). Any suggestions on changing the shape of the controller is appreciated.
```

---
## \#49 Posted by: Sander Posted at: 2017-05-01T17:50:54.090Z Reads: 321

```
Maybe change the placement for the antenna? Because it points up to the air not down to the board. Or flat.. If you make it coming out of the cylinder.
```

---
## \#50 Posted by: Print3r Posted at: 2017-05-01T17:52:53.579Z Reads: 323

```
The antenna currently can be rotated any which way for the moment - the long bit has a hinge point at the end. Will make it flat now.
```

---
## \#51 Posted by: Sander Posted at: 2017-05-01T17:55:53.014Z Reads: 335

```
Look what I found! You dont need no antenna anymore!
<img src="/uploads/db1493/original/3X/c/6/c6016da7b8f3d3f8dcc8eb681ef1a1611bcce8c9.jpg" width="503" height="500">
This is the long range module in smd! You can see it has an inbuilt antenna. It is listed on the same specs. So you should get 100 meter with no problem.
[NRF24L01 Long Range SMD](https://www.aliexpress.com/item/Free-Shipping-SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in/2022127731.html?spm=2114.40010508.4.27.OGF00a)

And the good thing I dont need to change the pcb because it has the same pins!

Im going to add a option in my app now. 
The option is Phone Location, or Board Location.
I think if I download the map and uses the phone location I dont need to use internet.
```

---
## \#52 Posted by: Print3r Posted at: 2017-05-01T18:18:11.352Z Reads: 314

```
I think that I will purchase 2 boards in september first with the smd antenna, test that to make sure it is safe and then purchase the larger antennas if ever the signal cuts out in testing. I am slightly dubious as to whether the smd antenna will allow for the same distance as the usual wifi antenna style (optimistic distance rating on the smd?), but if it is good enough following testing, I will go with that - gives more space for electronics and doesn't look like a middle finger!

Post pictures of your app/ pcb when you have made those changes - sounds great. I thought you said above that you were going to get rid of the gps in the transmitter? Or are you going to leave it in, but only use it if is triggered in the app?
```

---
## \#53 Posted by: Sander Posted at: 2017-05-01T18:30:59.223Z Reads: 303

```
You can choose to use the gps in board or the gps on your phone on the settings in the app. 
And I think the smd nrf24l01 long range is that good! Because it has Low Noise Amplifier and Power Amplifier. And if I use a UF capacitor to get rid of the noises in the power from the battery the range increases too!

You know the ESP8266 they have a ridiculous long range! They have only a pcb antenna. But the NRF Longrange smd has an external antenna cap, that improves. So it should work perfect! I will do some range testing with them in the future ;)

Yes I will show you images etc. Right know I need to add function like: You are not connected to bluetooth. Because sometimes I am wondering why I cant find the bluetooth device because I had my bluetooth turned off.
```

---
## \#54 Posted by: Print3r Posted at: 2017-05-01T20:09:59.449Z Reads: 294

```
Short animation of the controller without the long antenna!
http://a360.co/2oQEAuw
```

---
## \#55 Posted by: Sander Posted at: 2017-05-01T20:30:01.655Z Reads: 303

```
Looks good!
Btw you are right the phone is more accurate.
I get number that are much longer:
0.00000000000, 00.0000000000000
```

---
## \#56 Posted by: Sander Posted at: 2017-05-01T20:51:42.968Z Reads: 345

```
<img src="/uploads/db1493/original/3X/b/3/b3ebff3c229f00a6c3915770fa6d6eb8f180cefa.png" width="283" height="499">

<img src="/uploads/db1493/original/3X/e/2/e23c9dacfdaf74b1ebfd9e79de754b2937b34933.png" width="281" height="500">

**GPS Style:**

_Board:_
It uses a GPS that are connected to a processor in the electric skateboard, that sends the longitude and latitude via bluetooth to your phone. When the phone receive it, it calculates it and chooses the fastest route. Then the phone sends back the direction to the processor. The processor then sends it via a radio to the display on the remote. The remote shows where to turn, and when to turn in meters. 
Phone uses almost no power.

_Phone:_
It uses the Phones gps. Uses alot of power. It gets the latitude and longitude from the gps in the phone. And then it calculates the route to destination, sends back road direction via bluetooth. The processor forwards that data to the remote and display where to turn, and when to turn in meters.

_Follow Current Position:_
It follows your current position :)

-----

It displays the route on the phone(Not shown in picture because it shows my location). I will add more settings like accuracy of gps on phone, auto blinker, road type(Highway, Normal, bikepath, wallking path) and much more. Since the gps can calculate the time I can add various features like auto night light. You go on the phone/remote and choose the time when you want the lights to turn on. Like if the clock is 18:00 the light will turn on automatic, add a light sensor on it to so when you enter a tunnel with no light inside it the light on the board goes on.

_Bugs to be fixed:_
Timeout on making/refreshing routes.

Error: Error Domain=MKErrorDomain Code=3 "Directions Not Available" UserInfo={NSLocalizedDescription=Directions Not Available, MKErrorGEOError=-3, MKErrorGEOErrorUserInfo={
    GEORequestThrottleStateLevel = 0;
    GEORequestThrottleStateResetTimeRemaining = "0.5064319968223572";
}, MKDirectionsErrorCode=0, NSLocalizedFailureReason=A route could not be determined between these locations.}

To fix this I think I wlll need a delay, I hope I am right.
```

---
## \#57 Posted by: Sander Posted at: 2017-05-01T23:31:59.179Z Reads: 298

```
Looks like the Apple's API is shit! You cant send to many request and if you do it times you out for 6 second. So I will create the app again from the bottom, but this time I will use Google's API. I hear it doesn't time out like apple's api, which is good. So I hope this will work!
```

---
## \#58 Posted by: Print3r Posted at: 2017-05-02T06:10:55.908Z Reads: 311

```
Sorry to hear about apple maps api being annoying - you wouldn't expect it given how sleek they manage to make some apps!

[quote="Sander, post:56, topic:22055"]
The processor then sends it via a radio to the display on the remote
[/quote]

Is the first processor you are talking about in the board - nano in board is connected to vesc, bluetooth, GPS module and NRF. Seems like a lot for the bottom board to handle, given that you want it to send the data up from the VESC up without errors and send back throttle/ braking power without errors. But I may have misunderstood.
```

---
## \#59 Posted by: Print3r Posted at: 2017-05-02T06:12:41.844Z Reads: 290

```
The app looks great btw - very simple and sleek! Good luck with the Google API.
```

---
## \#60 Posted by: Sander Posted at: 2017-05-02T10:45:45.910Z Reads: 291

```
Yes the processor aka microcontroller ATmega32U4. The google api looks simple but there are no tutorials on direction but I will find a way! And in the API mananger you can limit how many request is allowed on a day or 100 seconds which is cool! Right now it stands on unlimited so there is hope! :)
```

---
## \#61 Posted by: Sander Posted at: 2017-05-02T11:15:08.019Z Reads: 262

```
YES! The Google API works! I haven't made the direction yet, but since I am using google's map you can download the MAP! To download the map you download the Google Map app and go to setting and download area nearby, when it is downloaded you can use it in my app so now you don't need internet to use the navigation which is awesome! or it should atleast because on you could do that on the Pokemon Go app. But on offline only the road route works, not the bike, walk routes.
```

---
## \#62 Posted by: Print3r Posted at: 2017-05-02T15:40:35.631Z Reads: 270

```
Are you designing your own board (for the chip)?! I like the offline functionality and the fact that you used Pokemon Go to explain how your app should work :slight_smile: ! I found that this tutorial explained well how to get a route using the API (https://developers.google.com/maps/documentation/), Google on the free plan lets 25,000 requests be made per day before you have to start paying!
```

---
## \#63 Posted by: Sander Posted at: 2017-05-02T17:17:41.810Z Reads: 289

```
Actually google gives you 150,000 request per day! if you contact them ;)
But the bad thing is I can only get direction by connecting to wifi. So the offline will not be available for now.

I can request as fast as I want with Google API which is amazing! If I create the arrow pointing the right direction everything gets more easier, because then I only need to request once. You see you are driving the wrong way when the meters goes up and the arrow is pointing behind you. 

I will try to make it saves it.
Well this is the data I get when I request:
https://pastebin.com/FgKg98iE
```

---
## \#64 Posted by: Print3r Posted at: 2017-05-02T19:11:23.276Z Reads: 314

```
Great that so many requests can be made! Wifi thing doesn't matter for the moment - first let's get proof of concept working, then improve and add extra functionality.

I agree with your point about the arrow, unless the road is winding and cuts back on itself - it will initially look like you are going the wrong way then you find out you aren't after checking your phone. Thought about having the arrow pointing at the current instruction's endpoint, but that will look choppy and will have the same problem if the road is winding. I suppose the rider knows that he/she should go straight on, unless told otherwise (in the outputted JSON there are maneuvers   ... "maneuver" : "turn-left",  ... so these could be displayed on the screen as temporary icons (like indicator lights) with metres to that maneuver on the bottom of the display) - see image. 

A more info button (for analysing stats when stopped) would also be nice - click the button and it goes to a list view of meters travelled, max speed, average speed, watt-hours/mile, watt hours used, estimated charge time (based on charge current and watt-hours used), battery voltage etc. For the more info, the fewest number of buttons I can think of is 3 --> one where if you click it, you go into more info (list) screen, click it again and you go back to the riding screen, another to scroll down and another to scroll up. 

I have put up a mock riding screen below (max 1 turn left/ right light will be displayed, but both are shown for placement) please give me your suggestions for how to change it. The green line is the edge of the screen (not to scale just roughly by eye guesstimated) and the italics are my thoughts for units decisions.
<img src="/uploads/db1493/original/3X/8/0/80309f3685f265ad03772bf9d976c51029476c2f.png" width="690" height="341">
```

---
## \#65 Posted by: Sander Posted at: 2017-05-02T19:38:38.962Z Reads: 315

```
Great idea! I wont have the following arrow, it was only an example for offline mode.
On the display where it display volt etc, I will make that they can change what to display in the settings.
Here are some of the arrow google uses and all the values for maneuvers:
**_Click Image For All Values(Image created in 2013)_**
<img src="/uploads/db1493/original/3X/9/4/949923ed22350c281f97dd18febcea68cf00efd2.jpg" width="100" height="500">
I will create a working version, right now I only get the route not the maneuvers.
```

---
## \#66 Posted by: Sander Posted at: 2017-05-02T21:29:57.922Z Reads: 290

```
Finally! It took ages to get the first maneuver! Now I get maneuver 1 by maneFirst[1],  maneuver 2 by maneFirst[2] etc. So now it is working now I need to test if it really works going for a walk brb ;)

Back from the walk:
Everything worked perfect! It told me to turn-left or turn-right which were right! Tomorrow I will add the distance. But if you are going the wrong way it doesn't tell you. If you were on the right track from the beginning I think it should not be a problem as long as it reroute you but when its only 1 road and you pass the only left it will keep telling you to go left.. So I need to make a counter of when the meters get  higher and higher when it has counter to 10 it will tell you, you are going wrong way, please turn around.
```

---
## \#67 Posted by: Print3r Posted at: 2017-05-03T06:24:39.502Z Reads: 279

```
Great work! Did you design the 'winning remote' in Fusion 360 - the handle of my remote looks rather big and I would like to compare it with a handle that has been tested and tweaked to the right size. Any more suggestions for the design of the handheld remote?
```

---
## \#68 Posted by: Sander Posted at: 2017-05-03T07:19:49.488Z Reads: 267

```
yed I designed the whole remote in fusion. I will give you the step file when i get home so you can compare it
```

---
## \#69 Posted by: Sander Posted at: 2017-05-03T13:19:13.512Z Reads: 267

```
Here is the link: http://a360.co/2qrWkMK
password is: oledremote
```

---
## \#70 Posted by: Print3r Posted at: 2017-05-03T13:21:27.854Z Reads: 260

```
Many thanks. Have you printed it and tested it sizewise? The level of detail in it is unbelievable - all the smds are also modelled!
```

---
## \#71 Posted by: Sander Posted at: 2017-05-03T13:33:52.575Z Reads: 259

```
The pcb is extracted from circuit maker but it doesnt show the solder pads so I created them. And the oled + potentiometer is readings from the real size value. So its correct sizewise! I have created with fusion before and printed so this should be sizewise, currently my 3d printer is working because I broke a part.. ;) I think I will make a Resin printer and print out the remote and create potentiometers.
```

---
## \#72 Posted by: rwxr Posted at: 2017-05-03T13:35:06.229Z Reads: 252

```
I've been following this thread for a few days without posting in it because I didn't want to interfere with your flow... I can't hold back any more.

Damn guys! This both looks and sounds awesome. I really hope you find time and inspiration to build prototypes of this. As far as remotes for the DIY-scene goes, we've been limited to GT2B and the Mini 2.4 and it's about time there's a new kid on the block.

Cheers!
```

---
## \#73 Posted by: Sander Posted at: 2017-05-03T13:39:49.133Z Reads: 253

```
I like people interfering so no problem there :D
The pcb is on the way and I recieved the parts of it today!

I will have the inspiration atleast because I am waiting for my parts to the electric skateboard, so I want a good remote with how I want it ;)
```

---
## \#74 Posted by: Print3r Posted at: 2017-05-03T14:29:51.342Z Reads: 250

```
Please do not feel that you are interrupting the flow of ideas @rwxr or anyone else who is reading this thread and has an idea. Though few people are discussing the remote, being developed on this thread, I have continued to reply publicly so that this controller can be made as good as it possibly can be - I am sure that other people will input valuable ideas based on their experiences and will value seeing the thought process behind decisions. Please reply with ideas of things you would like added to the code and changes to the design to make it look less bulky!
```

---
## \#75 Posted by: Sander Posted at: 2017-05-03T14:33:48.937Z Reads: 250

```
I agree!
10 char
```

---
## \#76 Posted by: Sander Posted at: 2017-05-03T14:39:45.016Z Reads: 262

```
Successfully retrieving distance and turns!
Btw I want the bluetooth in the remote and if we were going to have GPS in the board we could just send the float values via radio with no problems ;) It is easier to vizualize the elements if the bluetooth is connected to the remotes microcontroller.
```

---
## \#77 Posted by: Sander Posted at: 2017-05-03T15:19:18.166Z Reads: 287

```
<img src="/uploads/db1493/original/3X/a/f/af0326f0caed5cd561c92e1c5d3647b745e5cb0c.jpg" width="281" height="499">

I havent really done anything with the inteface on the app yet. 
You can see there are two labels saying turn-left. The first on is the first turn, the second one is the second turn.

I get the distance in string like this "50 m" and convert it to int and subtract 1-2 meters so yeah. It is working.
```

---
## \#78 Posted by: Sander Posted at: 2017-05-03T18:29:02.475Z Reads: 279

```
New bug:
The gps interferes the message from the phone.
> �c3�
> AcV�
> �,��
> AR,15
> �Y�
> ��S

When I unplugged it:
> AR,15
> AR,15
> AR,15
> AR,15
> AR,15

I think its the ESP fault, the esp isnt really created for this kinda work more wifi tho.
```

---
## \#79 Posted by: Print3r Posted at: 2017-05-03T18:31:22.401Z Reads: 285

```
I will not have any time to do more design work in the next couple of days/ weeks but here are some pictures of the remote, with the hole for the throttle/ brake/ reverse nub adjusted + @Sander's potentiometer and thumbstick. The rotational travel on the thumbstick is currently 50o (25o each way). Sorry that these are just plain screenshots not fancy renders, but I cannot find a way for fusion 360 to do a render when doing a cross-section:<img src="/uploads/db1493/original/3X/1/4/143ee5d3293df29c8167f4ff486572046fceb12a.png" width="690" height="320"><img src="/uploads/db1493/original/3X/1/c/1c37255b7f25b6bd394aaf48d592ff4c4f1faaa4.png" width="690" height="330">
```

---
## \#80 Posted by: Sander Posted at: 2017-05-03T19:43:03.810Z Reads: 277

```
**Update:**
The gps connected to Arduino sends the coordinates via bluetooth.
when the phone gets the coordinates it creates a path and sends back where to turn and meters to that turn.

The App works now in locked screen! So your phone don't need to be unlocked inside the app.

So it is working!
Refresh rate will be fixed later.
```

---
## \#81 Posted by: Print3r Posted at: 2017-05-03T19:54:46.051Z Reads: 263

```
Great work! I assume you got the ... [quote="Sander, post:78, topic:22055"]
ESP
[/quote]

bug fixed. Just checking that the board you have made has a voltage converter so that the whole thing can be powered off a 1s lipo. A low voltage warning should be added to the code for the lipo in the controller.
```

---
## \#82 Posted by: Sander Posted at: 2017-05-03T20:57:58.508Z Reads: 270

```
It operates on 2.5 voltage, thats the lowest for the ATmega32U4.

And the bug is when I send and recieve at the same time I get those weird values but that could be the ESP. 
I will not use the ESP, I am using it right now because I have no Arduino around. 

So when I get the UNO I will change the baudrate of the bluetooth from 9600 to 115200 so everything get processed faster which means faster refresh rate :) . The tracking is done! In the settings you can choose board gps, or the phones gps. And it seems like the board gps is more accurate it doesnt jump around like the phone does. The gps costed 24$ tho.

It does not send a request to google when the bluetooth is not connected.
When you are connected it sends request every second. 

On my ESP I receive the distance and which way to turn.

Here are some values recieved from the ESP from the phone.
> turn-right16 m
> turn-right16 m
> turn-right15 m
> turn-right17 m
> turn-right15 m
```

---
## \#83 Posted by: Print3r Posted at: 2017-05-04T06:02:35.429Z Reads: 270

```
That is good for the operating voltage! Might just buy one of these gps' for the moment, to see if the super-cheap gps' work okay (https://www.ebay.co.uk/p/?iid=272508603552&&&adgroupid=433339076421). Are you sure about the 2.5V, (arduino micro uses atmega32u4 and says min. ~6V ("The board can operate on an external supply of 6 to 20 volts. If supplied with less than 7V, however, the 5V pin may supply less than five volts and the board may become unstable."). Surprising that the gps on the board jumps around more than the phone!

Microcontroller	ATmega32U4
Operating Voltage	5V
Input Voltage (recommended)	7-12V
Input Voltage (limit)	6-20V
Digital I/O Pins	20
PWM Channels	7
Analog Input Channels	12
DC Current per I/O Pin	20 mA
DC Current for 3.3V Pin	50 mA
Flash Memory	32 KB (ATmega32U4)
of which 4 KB used by bootloader
SRAM	2.5 KB (ATmega32U4)
EEPROM	1 KB (ATmega32U4)
Clock Speed	16 MHz
LED_BUILTIN	13
Length	48 mm
Width	18 mm
Weight	13 g
```

---
## \#84 Posted by: Sander Posted at: 2017-05-04T11:33:41.214Z Reads: 238

```
That is arduino micro not my pcb. Mine is different. Mine works from 2.5-16V
```

---
## \#85 Posted by: Print3r Posted at: 2017-05-04T16:41:00.368Z Reads: 234

```
Great! I don't know if it would be possible for the average speed to be shown in settings - then input that speed in the app so ETA is more accurate. Maybe also add in the app, before trip is confirmed a screen that says you: will have ___miles left after this/ run out of battery with ___miles to go.
```

---
## \#86 Posted by: Sander Posted at: 2017-05-04T17:54:46.764Z Reads: 239

```
Thats pretty easy to do but first you need to know how much your battery is charged. But if you wanna know how much is charged you either have a bms that can tell you or I need to have a current reader when charging reading how much has been charged when battery is empty.
```

---
## \#87 Posted by: Print3r Posted at: 2017-05-04T18:03:55.391Z Reads: 243

```
Well, my idea was based on the VESC outputting over uart (among other things) the total battery voltage and Watt-hours used. So, the user inputs the watt-hours of his battery and max voltage in app settings, then watt-hours left can be calculated from starting watt hours (look at voltage to estimate starting watt-hours in battery), then subtract the watt-hours used (from VESC). The Wh/mile can be calculated every 1/10 mile by putting the value of watt-hours at the start in a variable and putting the value of watt-hours at the end of the 1/10 mile in a variable and finding the difference. Then *10 to get a number and add the string "Wh/mile".
```

---
## \#88 Posted by: Sander Posted at: 2017-05-04T18:10:58.479Z Reads: 268

```
Yes but the voltage jumps from 44.4 to 44.2 to 44.4 to 44.2 etc. So it would be better if I created a current reader on my pcb. So when you charge the board the VESC turns on gives power to the pcb and it reads. With the VESC I can see how much has been drawn so if I have a value like: unsigned long charged = 0;
So when the current reader reads current you calculate it and make it into mAh. So for my board it will be 12000mah. 

With the VESC I can use the Amp/watt hour to remove the mah. And when regenative braking it tells you "You have regenerated 15 mah" in the Stats sections.

Here is a current sensor supporting 50A, 100A, 150A and 200A.
But I dont know what is the max voltage or does it have it?
http://www.ebay.com/itm/50A-100A-150A-200A-Bi-Uni-AC-DC-Current-Sensor-Module-arduino-compatible-/111689533182

Here is an example to measure the charged mah's.

> float watts = amps * batteryVoltage;

> sample = sample + 1;

> msec = millis();

> time = (float) msec / 1000.0;

> totalCharge = totalCharge + amps;

> averageAmps = totalCharge / sample;

> ampSeconds = averageAmps*time;

> ampHours = ampSeconds/3600;

> wattHours = batteryVoltage * ampHours;

Since I have no boards to use the oled on. I will create a "arduino simulator" in processing for the OLED. When the ESP get value from the bluetooth it send the value with Serial to the Processing.
```

---
## \#89 Posted by: Print3r Posted at: 2017-05-04T18:42:40.308Z Reads: 261

```
Slight problem:
<img src="/uploads/db1493/original/3X/f/1/f19727c75106eccd16875e1a6a117e07774d44eb.png" width="571" height="500">
```

---
## \#90 Posted by: Print3r Posted at: 2017-05-04T18:49:14.323Z Reads: 255

```
My board will be a 8s that is split into two 4s (same mah) with the on/off switch. Now the two batteries are split up, I can charge both the cells in parallel. The problem with this and your planned setup is that the vesc cannot be on whilst charging (not a complete circuit for battery input). However if you use a lipo/liion charger you can see the amount of charge put in the batteries (mah). So, if the user inputs these charge mah values into the app before riding, it will work the same, just without so much maths and finding a chip with the right specs!
```

---
## \#91 Posted by: Sander Posted at: 2017-05-04T19:25:30.819Z Reads: 247

```
so 28V id max?
```

---
## \#92 Posted by: Sander Posted at: 2017-05-04T21:45:13.704Z Reads: 270

```
Here is it running on my "OLED Simulator". Its the ESP that are sending it values like it will do to the OLED.
https://www.youtube.com/watch?v=CAvZkdqqaD8&feature=youtu.be


You are wondering why does it randomly changes directions? Its because I am standing near a cross point. Its a turn to right at the end of the road. PS I am moving around.
<img src="/uploads/db1493/original/3X/5/f/5fae77c62ba8780cf87174be00ea443945e26623.png" width="515" height="500">

_Bugs/Things to fix:_
- When my phone is locked our at home screen it "forgets" to send the distance.
- Update rate
```

---
## \#93 Posted by: Print3r Posted at: 2017-05-05T06:44:56.359Z Reads: 243

```
liion so 28.8V nominal voltage, 33.6V fully charged (will only charge to 32V to extend battery life), 20V fully discharged but would only discharge it to 26/25V (to extend life of batteries). Under my board I will also have a 5000mah 5V battery pack to charge things like my phone when not riding and power the processor whilst riding. Your directions look good but don't know why the distance was increasing as you approached the crossing! The signs look clear though and the distance doesn't update so often that it is distracting. I don't what the AR and AL things were (0:03 and 0:16) on the simulated OLED - think it was that there were 0m left to that direction?
```

---
## \#94 Posted by: Sander Posted at: 2017-05-05T06:49:36.529Z Reads: 244

```
You can see the picture above. It creates the shortest route for you. When I am standing on the red dot it switches. The one route is 15m to the right the other is a long 54 meter road with turning to the left. 

You could be right with the 0 meter thing but I doubt it. When I lock my phone it only sends the meteres after 3-5 bluetooth package. It sends like this when its locked:
> AR,15 M
> AR
> AR
> AR
> AR,15 M

AR is for Turning right, AL is Turning left.

Because I wasnt on the road it changed direction but when I stand on the road it is stable does not change routes ;)

I will make a video when I am on the road. So you can see it is working perfect.
```

---
## \#95 Posted by: Print3r Posted at: 2017-05-05T06:55:00.834Z Reads: 223

```
That sounds great and makes much more sense than my theory! Weird that the phone just doesn't send metres for 3-5 packets. Can't wait to see the video on the road when you get it filmed - how do you take a video of this simulation? Are you walking with your laptop open in front of you :slight_smile: !?
```

---
## \#96 Posted by: Sander Posted at: 2017-05-05T06:57:34.656Z Reads: 241

```
I will have my ESP connected to a Nexton display because I have no oleds working. I will only have the things I will have in my board ;)

Btw here is a current sensor rated 51V Max and 90A Max:
https://www.sparkfun.com/products/9028

And here is a [sketch.](http://cdn.sparkfun.com/datasheets/Sensors/Current/CurrentSenseDemo.pde)
```

---
## \#97 Posted by: Print3r Posted at: 2017-05-05T07:10:53.115Z Reads: 237

```
The price for me is not a problem, but I like sourcing components cheaper and making things smaller ... so have read up on the way the voltage is measured: "This is a small voltage and current sense PCB. DC current is determined by measuring a voltage drop across a pair of parallel shunt resistors, then converted to a final analog voltage output by the TI INA-169. Voltage sense is accomplished by scaling to 3.3V ADC range by a precision resistor divider."
So if you could integrate this pcb into your board then all that needs to be done is: take inspiration from (replicate) the pcb layout of this board on yours with the processor,  buy a TI INA-169 ($2) and some SMD resistors. I looked for the same board (but cheaper) on ebay than that on sparkfun but couldn't find one :( !
```

---
## \#98 Posted by: Sander Posted at: 2017-05-05T10:42:00.440Z Reads: 232

```
I could probably make one for 5-8$ in built in the big pcb.

I want to create a pcb with dual vesc, with current sensor and the arduino reciever.
```

---
## \#99 Posted by: Print3r Posted at: 2017-05-05T10:45:35.649Z Reads: 239

```
I don't know how to solder large smd chips like on the vesc, but suppose it will be an opportunity to learn. If you could also do a single vesc pcb + current sensor + arduino receiver that would be great. I will set up this evening a vote for who would be interested in buying a dual vesc pcb vs single vs only the arduino receiver and current sensor vs not interested.
```

---
## \#100 Posted by: Sander Posted at: 2017-05-05T11:19:40.248Z Reads: 256

```
Soldering is bad. Hot Air is the best way to do if you dont have a reflow oven. First you order a pcb. Then the stencil for it. Using solder paste over the stencil so the solder pads get solder on it. Place the smd components on the solder pads. Heat the pcb with the hot air gun and watch the magic :)
```

---
## \#101 Posted by: Sander Posted at: 2017-05-05T13:48:20.220Z Reads: 257

```
Now the transmitting in locked screen / home screen is now fixed!
All I now need to do is make a faster refresh rate like every 100ms not every second.

I added if your position does not change it wont send a request nor if you aren't connected to bluetooth.

<img src="/uploads/db1493/original/3X/e/3/e3104307222991606ea0118e9c4a3e7e9d781d5f.jpg" width="375" height="500">
```

---
## \#102 Posted by: Print3r Posted at: 2017-05-05T16:57:25.869Z Reads: 258

```
Would you want a board pcb with an integrated:
[poll type=multiple min=1 max=2 public=true]
* Single VESC + current sensor + arduino receiver
* Dual VESC + current sensor + arduino receiver
* Current sensor + arduino receiver ONLY
* Not interested in such a large remote
* Other (please comment)
[/poll]

Would you want the pcb to:
[poll name=poll2 max=5 public=true]
* come with components and you have to put it together
* come with all the components already attached (plug and play)
[/poll]
```

---
## \#103 Posted by: Nordle Posted at: 2017-05-05T19:44:26.586Z Reads: 233

```
I would like to get a TX/RX pcb combo where i could connect a pot and maybe 1-2 buttons for reverse/cruise control, maximum a led that shows battery status. That all as small as possible;) All the fancy stuff should be optional and on smartphone.
Would like to build my own remotes but im not able to smd solder or write code.
```

---
## \#104 Posted by: Print3r Posted at: 2017-05-06T07:03:51.885Z Reads: 231

```
I believe you are looking for a remote like this - https://www.electric-skateboard.builders/t/ultimate-vesc-controller-with-oled/21922. The code for it is here https://github.com/RollingGecko/ArduBoardControler. RollingGecko has made his remote currently work this way:
"I use a 2 axis joystick. Left and right is to flip though different views on the display.
Forward is accelerating. backward is variable breaking.
One button is used to change direction. Pushing it once is for backwards . Pushing it again is back to forward. Accelerating and breaking remains.
The second button is used for speed control. It will keep the rpm on a constant level as long as you push it"
```

---
## \#105 Posted by: Nordle Posted at: 2017-05-06T08:25:39.332Z Reads: 226

```
No, i want a bit more finished product, his code didnt work for me, or it was the chinese stuff i ordered. Anyways i dont want to fiddle with these things anymore.
```

---
## \#106 Posted by: Print3r Posted at: 2017-05-06T08:48:22.208Z Reads: 246

```
I think that @lox897 is testing RollingGecko's code and is looking to make a compact remote (exactly as you have described) that works well. He seems to want to make a few working prototypes though before selling a fully made controller in the $30-40 range (he hopes). If you do not want the screen, you can simply ask him to not include it in the product he sends you. The reason I am pushing you to that thread is that the remote you are looking for has already been made (nunchuk), one with slightly more features is being prototyped (www.electric-skateboard.builders/t/ultimate-vesc-controller-with-oled/21922/70) and the one under development here is going to have loads of features. In my eyes, this is asking a smartphone company to make a nokia 3310 because it is smaller - it is a very different product to the one the smartphone company is developing and is already available!

On the other hand, given that there will be an app to go with the remote, a lot of the fancy stuff should be done in the app to make the remote processor run faster and the remote ui less complicated. 

So if you want a finished compact remote, get a nunchuck remote or wait for @lox897 to finish making RollingGecko's code run super smooth on his remote. If you want a slightly bigger, more featured remote, wait for this one to finish being developed, then tested, then sold. I hope this makes sense :) - I didn't mean for it to be so long!
```

---
## \#107 Posted by: Sander Posted at: 2017-05-06T09:33:11.855Z Reads: 224

```
Well this remote will not be bigger in size it could be smaller in size. I think about we selling it in different sizes ;)
```

---
## \#108 Posted by: Print3r Posted at: 2017-05-06T10:22:29.882Z Reads: 242

```
I would love to sell the remote in different sizes ... it is just the more inventory you have, the more all items cost (for each different size you have to make a different case, different screen, different code - a different sized screen has more space to put new stuff on. Then, when you manufacture it, you have to buy more products so that you can keep every size of controller in stock in EU/ America and ship it to the customer faster. We will have to see if interest for more sizes is very high, before making more sizes - there is no point selling something that already exists as those who need that can just go for that (unless a brand name becomes huge and then people go for the most 'reliable' company's product). **Please vote in the poll above if you haven't already to see interest. I will also add a poll here for different screen sizes.**

What screen size would you prefer:[poll]
* 1.3" (128*64) (http://www.ebay.co.uk/itm/New-1-3-SPI-Serial-128X64-OLED-LCD-Display-Screen-Module-for-Arduino-UNO-R3-51-/292036322441)
* 0.96"(128*64) (http://www.ebay.co.uk/itm/3-5V-0-96-12C-Serial-128X64-OLED-LCD-LED-Display-Module-for-Arduino-White-fo/152463801223)
* 0.91"(128*32) (http://www.ebay.co.uk/itm/0-91-IIC-I2C-SPI-Serial-128x32-White-OLED-Digital-Display-Module-Screen-Board/311829931498)
[/poll]
 
I will start buying components this weekend - SPI screen (http://www.ebay.co.uk/itm/New-1-3-SPI-Serial-128X64-OLED-LCD-Display-Screen-Module-for-Arduino-UNO-R3-51-/292036322441), 800mah lipo (linked previously), lipo usb charger, super cheap gps, already have potentiometer, @Sander is working on pcbs, chips needed (for receiver + vesc + transmitter - please send links). Is the NLF going to be integrated or should I buy the boards from aliexpress? Have you decided on the ESP vs bluetooth - send links for which I should buy?
```

---
## \#109 Posted by: Sander Posted at: 2017-05-06T10:45:45.649Z Reads: 220

```
I will not use the ESP, I said its the only board I have laying around for testing the bluetooth etc. The ESP is shit it always crashes. I will use a standard microcontroller. I will use the bluetooth. PS why are you using SPI screen? I am using I2C.

Btw Creating the most reliable controller in the world is my goal :sweat_smile:

Actually the max voltage for my board is 6.3V.... Because I suddenly bought a Ceramic Capicitor that has 6.3V max. All my other parts has from 150V-16V.. but that gets fixed if I buy the same cap only with 16V.

And with the sizes I meant the remote not the screen but oh well ;)
```

---
## \#110 Posted by: Print3r Posted at: 2017-05-06T13:33:18.984Z Reads: 231

```
I thought so for the ESP, but was just checking. I just used the cheapest screen I could find, found a new one that uses I2C. I will be either supplying the board with 5V or 1s lipo so shouldn't need the extra voltage but good to have it I suppose. I am also eager to make this the most reliable controller in the world (the PA is overkill but should eliminate any chance of no signal!). I didn't really know how else to quantify the size of the remote - the extra size comes from the screen - the 0.7" or 0.91" could be integrated on the side of a winning-style remote and you just ride with the thumbwheel to the side and the screen pointing to your face, but that is a really uncomfortable position to hold. I may try and make the screen be pushed up rack and pinion style by a servo - when the screen is stored the remote will be smaller. The problem that comes to mind with that is water ingress between the edge of the screen and the edge of the slot. If you have thoughts on making the remote smaller please tell me! I have put the links for stuff I will buy below. Could you let me know of what chips and capacitors and resistors I will need for the transmitter and receiver when you are done with the pcb. If the pcbs are not too big I know someone who can make a tester one the DIY way.

**I2C 1.3" screen** (www.aliexpress.com/item/1-3-White-IIC-I2C-Serial-128X64-OLED-LCD-Display-Screen-Module-For-Arduino/32716234430.html)
**Bluetooth HC-06 module** (www.ebay.co.uk/itm/HC-06-Bluetooth-Wireless-Serial-RF-Transceiver-Communicate-Module-for-Arduino-BG/111871749220)
**Pack of 5 Battery+usb charger** (www.banggood.com/5X-Eachine-3_7V-500mah-Lipo-Battery-with-1-to-5-USB-Charging-cable-p-1000438.html)
**Very cheap GPS** (www.ebay.co.uk/p/?iid=272508603552&&&adgroupid=43333907642)
**NRF*2 (with PA and smd antenna)** (www.aliexpress.com/item/Free-Shipping-SMD-NRF24L01-1100-meter-long-distance-NRF24L01-PA-LNA-SMD-wireless-modules-1100meters-in/2022127731.html)
```

---
## \#111 Posted by: Sander Posted at: 2017-05-06T14:10:33.891Z Reads: 217

```
the bluetooth is hm-10 module btw(4.0BT for iOS/Android). With the water protection I think I will use silicon on the edges to get it 100% water proof. 

I can give you the BOM list when I am sure everything is working ;)

You are right about it can be ucomfortable to look at. I will find a way to fix it top.

I think I will go with a bit expensiver gps because the cheap one likes to jump around when you are moving
```

---
## \#112 Posted by: Sander Posted at: 2017-05-06T15:02:22.232Z Reads: 219

```
YES I finally found a uno that worked! All my others are burnt. 
So now the bluetooth should work perfect.

OKEY HOLY COW! I got it working with only 5MS DELAY!
But when I add the GPS in the code the bluetooth does not work..
```

---
## \#113 Posted by: Print3r Posted at: 2017-05-06T17:32:30.155Z Reads: 232

```
I will stick with stick with the super cheap gps as I will mainly use the phone's gps. I will likely use the gps for some other project! Ok for the HM-10 module so 2 of these (http://www.ebay.co.uk/itm/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module-Arduino-Android-IOS-/272393169365). I may have found a solution for the water problem now you mention silicon, it may also allow the display part to be modular. I will post it as soon as it is done. Does anyone know how the flip up nintendo/ old nokia screens stayed in place (a flip-up screen was my second idea).
```

---
## \#114 Posted by: Sander Posted at: 2017-05-06T17:45:38.671Z Reads: 215

```
Or this [HM-10](http://www.ebay.co.uk/itm/HM-10-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module-Arduino-Android-IOS/191918243441?_trksid=p2047675.c100623.m-1&_trkparms=aid%3D222007%26algo%3DSIC.MBE%26ao%3D2%26asc%3D43781%26meid%3Db76bd4c209d145b08fb45f9d291bf259%26pid%3D100623%26rk%3D3%26rkt%3D6%26mehot%3Dag%26sd%3D272393169365) with some protection. 

Now the bluetooth and gps works perfect! It sends and recieves on 10 milliseconds. That should be fast enough. The flip up screen I have no idea.
```

---
## \#115 Posted by: Iam319 Posted at: 2017-05-06T18:09:50.432Z Reads: 206

```
Any idea when this will be ready for sale?
```

---
## \#116 Posted by: Sander Posted at: 2017-05-06T18:12:00.608Z Reads: 208

```
in 1-2 months depending on which time I get my parts.
```

---
## \#118 Posted by: Print3r Posted at: 2017-05-06T18:33:25.581Z Reads: 210

```
I am quite confused by what that reply meant @Sander (was it accuracy of gps?)!  :slight_smile: )

Shipping is not quick when things come from China!
```

---
## \#119 Posted by: Sander Posted at: 2017-05-06T19:14:09.516Z Reads: 221

```
I figured it out, thats why I deleted it. 

Yeah from china things takes time... 3 weeks.
Well I only ordered 10 of the LNA, PA, NRF from china. The only place they had them.
```

---
## \#120 Posted by: jackw Posted at: 2017-05-08T20:43:17.501Z Reads: 212

```
What do you think about a deadman switch? Would it be a case of interrupting the pot wires with a momentary switch?
```

---
## \#121 Posted by: Sander Posted at: 2017-05-08T20:48:26.775Z Reads: 223

```
Hmm what do you mean with a deadman switch? Do you mean a momentary push button for turning off and on the power?
```

---
## \#122 Posted by: jackw Posted at: 2017-05-08T20:52:20.029Z Reads: 236

```
Like the boosted board and others, basically a switch/trigger that you need to hold down in order for the thumbwheel to be active, so a kind of safety switch so that if you let go of the trigger the board doesn't fly away, and stops any accidental hitting of the thumbwheel.
```

---
## \#123 Posted by: Sander Posted at: 2017-05-08T21:03:09.192Z Reads: 240

```
Ahh yeah I get it great idea! :D I will add that to the remote in the future! 
Right now I need to create a stable firmware to run it on when I receive my pcb ;)
<img src="/uploads/db1493/original/3X/4/7/47a40bbac7c8b5e930a0e2fd76f42345d7b6576d.jpg" width="690" height="361">
```

---
## \#124 Posted by: Print3r Posted at: 2017-05-09T05:48:37.099Z Reads: 243

```
That's a great idea to include an arm switch/ deadman switch @jackw and to also use that switch to select items in the menu @Sander! If there is a free digital input pin on the atmega in the remote, I think the momentary (arm/ deadman) switch should be connected from 5V to that - if the switch is in series with the pot and it is in reverse mode (and pulling back decreases the resistance and means accelerate back when in reverse mode), the board would shoot towards you when the button is pressed. I will explain this with some diagrams later as I can't explain it will with words! Good luck with the firmware @Sander!
```

---
## \#125 Posted by: Sander Posted at: 2017-05-09T06:38:25.358Z Reads: 237

```
You know you can connect the button with a Digital Output to Ground that results in HIGH or LOW ;)
```

---
## \#126 Posted by: Sander Posted at: 2017-05-09T19:39:27.454Z Reads: 253

```
<img src="/uploads/db1493/original/3X/c/0/c0129eac9949e6fee6962a55e07aca02a6d4de85.png" width="690" height="361">

And with the yellow there will be cruise control/horn.
When you are either breaking or have released the throttle it will honk. 
To activate the cruise control you first have to press in the "Deadman switch" to activate the throttle if not it will honk. To honk you just release the "deadman switch".

So I think I will create a pcb where the buttons are mounted on it or I will do the easy way:<img src="/uploads/db1493/original/3X/2/9/29f7bc47c112c872ccd5ae1782b54e6b1b631d47.png" width="391" height="500">
The red is the switch and the black is the wall around it.
Do the same way with the buttons.
```

---
## \#127 Posted by: Tomer Posted at: 2017-05-09T20:00:40.754Z Reads: 243

```
I think it will be better to have a specific button for horn. The way you described it, in my perspective, is not very convenient when you ride in high speed and something happen therefore you need to horn, it will be too confusing in those critical moment (I might be over dramatic lol).
```

---
## \#128 Posted by: Sander Posted at: 2017-05-09T20:20:16.632Z Reads: 242

```
Good thinking! If I just "remove" the cruise control for now and just have the horn function instead?
I think these will be some good horns, they are small and loud:
http://www.ebay.com/itm/SUPER-LOUD-BLAST-TONE-GRILL-MOUNT-12V-ELECTRIC-COMPACT-CAR-HORN-335-400HZ-RED-/112357152241?hash=item1a290215f1:g:d6YAAOSwvzRXxVUZ&vxp=mtr
```

---
## \#129 Posted by: Tomer Posted at: 2017-05-09T20:23:12.258Z Reads: 236

```
I think that cruise control is more useful than horning. I will rather having cruise control ability instead of horn, I will just scream as loud as I can to who's in front of me :grinning:

Can you add another button or there is no enough room?
```

---
## \#130 Posted by: Sander Posted at: 2017-05-09T20:26:19.976Z Reads: 245

```
Plenty of room. But since the remote is so small the position where the cruise control/horn is were pretty hard to access.

I need to find better places to add the buttons ;)
```

---
## \#131 Posted by: Tomer Posted at: 2017-05-09T20:37:24.442Z Reads: 242

```
This is what I think the buttons should look like.

<img src="/uploads/db1493/original/3X/2/2/22a5e92ffbdef33638547b2cc6e7b2af89b836b4.png" width="690" height="361">
```

---
## \#132 Posted by: Benja_man Posted at: 2017-05-09T20:41:02.881Z Reads: 232

```
I think the horn placed there @tomer is useless. It's impossible to reach when you need it if you have a finger stuck in the hole.
```

---
## \#133 Posted by: Tomer Posted at: 2017-05-09T20:42:50.919Z Reads: 229

```
@Benja_man You probably right, I never held the Winning remote in my hand so I don't know... Is it possible to make the throttle clickable to enable the horn?
```

---
## \#134 Posted by: Sander Posted at: 2017-05-09T20:42:55.454Z Reads: 231

```
I see, I will need to change the layout of the remote in the future for better grip and button access.
```

---
## \#135 Posted by: Sander Posted at: 2017-05-09T20:43:29.462Z Reads: 228

```
the throttle is clickable from the start of ;)
But I will need the "deadman switch" thing for enabling the potentiometer.

With the horn again. Some countries need you to have horn and lights for legal road use etc.
```

---
## \#136 Posted by: lox897 Posted at: 2017-05-09T20:49:16.872Z Reads: 228

```
Oooo oooo oooo I know! When you horn you pretty much would be in a situation where you need to brake right?!?!? So why not put the horn button where the throttle would be when braking? So you'd press the throttle in and it would brake? Idk this might not be the best idea... Thoughts?
```

---
## \#137 Posted by: Sander Posted at: 2017-05-09T20:56:07.585Z Reads: 228

```
hahaha yes! That would be funny if you were breaking and suddenly a loud noise comes out of nowhere!

Good thinking! but not the best idea, I think the best way is to have a seperate button for horning ;)
But giving it a second thought if you break very fast I can do it activate the horn? It seems not so dumb at all but you need to break then to activate the horn... You rather will have some speed not stand still and honking.
```

---
## \#138 Posted by: lox897 Posted at: 2017-05-09T21:02:22.687Z Reads: 228

```
Yes good idea. If the brake goes quickly enough maybe it horns and brakes. How would this be done? Is there code that allows you to check how quickly something changes?
```

---
## \#139 Posted by: Sander Posted at: 2017-05-09T21:05:11.799Z Reads: 228

```
Yes its easy... I do a time reading(ms), if throttle was 0 or 50 and drawn to -80 =< -100 on 100-500ms it will honk.
```

---
## \#140 Posted by: Print3r Posted at: 2017-05-10T05:59:11.730Z Reads: 250

```
Maybe make this feature be 'turn-offable' in the app/ on the remote - it reminds me of a Topgear episode where the horn was attached to the brakes and that did not end too well. I will print out your initial remote this afternoon (printing 40 18650 models atm) and will see how comfortable it is/ where  more buttons could go. As everyone really likes the benchwheel style remote (it is super compact), I have been thinking of how a 1.3 inch screen could be mounted to it. The idea I am currently going to go with is a flip out remote like on a camcorder:<img src="/uploads/db1493/original/3X/f/1/f13c527f3bf3d0c1e343943105f285146070361f.png" width="690" height="361">
I will measure up the pcb holes location on the remote once it is printed and see what is the larges screen possible with the space available/ how much it has to be expanded to accomodate a 1.3 inch screen. I have put the hinge so far up in the diagram so when the screen is swung out to perpendicular, it does not interfer with your finger location/ ability to hit the many new buttons (thank you for all the new suggestions!). 

As far as I can understand, duty cycle to the vesc can be adjusted from 100% (full acceleration) to -100% (full brake). @Sander Could you make the spring loaded pot go from -100 to 100 duty cycle (the variable braking I was talking about earlier but couldn't explain well!). It would also be interesting to be able to adjust the max and min duty cycle on the app/ controller - so that you don't get flung off the board because at 100% the acceleration is too fast or at -100% the braking is too hard.
```

---
## \#141 Posted by: Sander Posted at: 2017-05-10T06:24:38.829Z Reads: 245

```
Great idea!
The 100 and -100 is the ampere to give the motors.
When its 100 its not fully 100 amps its doing some math something like: (ampere * 2) / 100

Yes I will have the fast feature of changing modes and an other feature like they choose the max speed and acceleration speed(ms)
```

---
## \#142 Posted by: Print3r Posted at: 2017-05-10T06:26:50.845Z Reads: 230

```
Max speed/ acceleration would be a super cool feature!
```

---
## \#143 Posted by: Print3r Posted at: 2017-05-11T11:08:04.039Z Reads: 258

```
Based on the large amount of people who have expressed their preference for a small remote, I have quickly made some renders of a 'winning' style remote with a 1.3" Oled screen that flips up from the side. I have yet to work out a way of getting the screen to stay up -  if you have any ideas please suggest them. In the renders I have not yet put the various buttons in as I wasn't sure if their position/ how many was finalised. The screen is just some dummy text and placement - please suggest what and where stuff should be on the screen. As the screen is 'flip up', you will also be able to ride with it stored. Maybe for flipping the screen, a servo with a gear instead of a servo horn could be used, then put another gear on the screen holder that rotates. I have decided also to make the hinge run along the side of the screen pcb (long side nearest thumbstick) as it will be stronger that way. I will test the size of the controller tomorrow (printing now) as ideally for the larger screen it would be 10mm bigger (if not the pcb would have to be sanded wherever possible)!

Snazzy renders:
<img src="/uploads/db1493/original/3X/5/1/516fa136299707579af771484fd845cc7d9d513f.png" width="400" height="500">

<img src="/uploads/db1493/original/3X/1/e/1e620756e5bebfd2699191664c71a706afbe7d35.png" width="462" height="499">
```

---
## \#144 Posted by: Print3r Posted at: 2017-05-12T16:27:07.293Z Reads: 240

```
I tried printing the remote yesterday, but half-way through the print, ABS spilled out above the nozzle -  print failed so will try that again on Monday/ Tuesday depending on when I get it cleaned up and the nozzle tightened. Luckily, before the print failed, the thumbstick finished printing. The size of the main part of the thumbstick's seems fine (don't have the main part of the remote to test it on) but the stick that attaches to the potentiometer is too thin (3 layers) and will be thickened. How is the code coming along @Sander?
```

---
## \#145 Posted by: Sander Posted at: 2017-05-12T17:32:46.553Z Reads: 234

```
Haven't really worked much more on the code this week, no time.
But I will work a bit more this weekend maybe ;)
```

---
## \#146 Posted by: Print3r Posted at: 2017-05-14T09:19:45.184Z Reads: 231

```
If you could integrate a on/ off mosfet switch into the board pcb that would be very cool. Ideally for my setup, I am looking for a switch that could isolate two connections. If the pcb design is already done, I will make do with 2 xt-90 loop keys.
```

---
## \#147 Posted by: Sander Posted at: 2017-05-14T10:10:12.171Z Reads: 221

```
I think I can manage that ;)
```

---
## \#148 Posted by: Print3r Posted at: 2017-05-14T10:14:41.364Z Reads: 221

```
VESC 6 is really confusing me - are Vedder's files on github the vesc 6. When is the VESC 6 being released? Now that Trampa has trademarked the VESC name, what do other sellers now call the VESCs they are making!
```

---
## \#149 Posted by: Print3r Posted at: 2017-05-14T10:16:05.235Z Reads: 227

```
NVM found the latest schematic as of may 11 2017 at the bottom of (http://vedder.se/forums/viewtopic.php?f=6&t=590&start=10).
```

---
## \#150 Posted by: Sander Posted at: 2017-05-16T11:29:59.878Z Reads: 218

```
Time to write the code from scratch with some libraries.
I will create the menu and the direction thing now.
```

---
## \#151 Posted by: Print3r Posted at: 2017-05-16T15:43:09.892Z Reads: 214

```
u8glib for the screen?
```

---
## \#152 Posted by: Sander Posted at: 2017-05-16T16:31:25.971Z Reads: 223

```
I use adafruit right now... I know the u8glib uses less space.

I have always trouble with uploading bootloaders.
I recieved the pcb today and still havent been able to upload the bootloader.
I get error signature 0xffffff...

So it might not work but if I do the old way, buying a lenardo and taking that chip off and take it on my pcb.
```

---
## \#153 Posted by: Print3r Posted at: 2017-05-16T16:34:55.487Z Reads: 216

```
Fair enough - adafruit was my go to until I learnt u8glib uses less space. Is the arduino bootloader on the chip - when you buy the leonardo it will come preinstalled but maybe not when you just buy the chip? BTW why are you using the atmega 32u4 - it is v.difficult to find it in chip form (not on a board) on the internet.
```

---
## \#154 Posted by: Sander Posted at: 2017-05-16T17:20:15.648Z Reads: 214

```
I dont know, It looked cool....
```

---
## \#155 Posted by: Print3r Posted at: 2017-05-16T17:24:44.964Z Reads: 219

```
lol ... because ... science
```

---
## \#156 Posted by: Print3r Posted at: 2017-05-16T18:22:32.160Z Reads: 231

```
You fixed the problem yet?
```

---
## \#157 Posted by: Sander Posted at: 2017-05-16T19:34:37.538Z Reads: 253

```
<img src="/uploads/db1493/original/3X/7/c/7c46b7e15d3f5f90cf62bb45e1ad3b0597928ea8.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/c/d/cdbd5e2ec36fa39ae315cf3b46057506f094b5f6.jpg" width="375" height="500">

The problem is when I try to install the bootloader it does not work...
It only says unknown signature.

When I connect the PCB with a usb to the pc it comes up as a 'Unknown Device' because I have of course no bootloader on it... It could be the Arduino UNO's fault?

<img src="/uploads/db1493/original/3X/5/d/5d672a9f7a8daa6630f6fd104dc00ad35d12d8ea.jpg" width="375" height="500">
```

---
## \#158 Posted by: Sander Posted at: 2017-05-16T19:46:48.957Z Reads: 232

```
I think I have found my problem!

> HWB: low: 0xff, high: 0xd8, 

When the HWB is LOW it gives out 0xff in bits and that is what the signature I get.
I have read when the HWB is set HIGH it gives something like this out 0xd8.
```

---
## \#159 Posted by: Print3r Posted at: 2017-05-16T20:00:11.950Z Reads: 228

```
Hope that was the problem that was causing the error message ... if not I remember that when uploading bootloaders, you sometimes need to hold down reset button/ have a capacitor somewhere.
```

---
## \#160 Posted by: Sander Posted at: 2017-05-16T20:09:43.030Z Reads: 234

```
I dont know how I make the HWB high? Connect to ground or vcc??
Yeah and any capicator higher then 1UF.

I think I have an idea, I will do more tomorrow.
```

---
## \#161 Posted by: Sander Posted at: 2017-05-17T11:46:11.667Z Reads: 244

```
The solder pads are so bad quality!
They break of so easily, I have a hard time connecting to the HWB pin.

Well I gave up on that, went to my backup plan.
I have bought a Arduino Micro I will use as a "bootloader board" along with the shaft for my 3d printer.
It should arrive in a few days ;)
<img src="/uploads/db1493/original/3X/e/9/e9af6d4e869ba7a624d6d81f190f8dba4d2445d6.jpg" width="500" height="500">
```

---
## \#162 Posted by: Print3r Posted at: 2017-05-17T12:11:55.846Z Reads: 232

```
Why not make a pcb that you can solder an arduino pro mini (http://www.ebay.co.uk/itm/New-Pro-Mini-atmega328-Board-5V-16M-Arduino-Compatible-Nano-NEW-/141695440186?hash=item20fdb4d53) to - this would avoid bad solder pad problems as the chip comes pre-mounted on the board? I am hopefully going to get the controller printing tomorrow (if I get the printer nozzle unclogged), so should be able to say if the controller could be made a bit bigger (like the benchwheel remote). Hope that the bootloader board solves your problems!
```

---
## \#163 Posted by: lox897 Posted at: 2017-05-17T12:47:27.224Z Reads: 221

```
How do you guys display variables with U8Glib?
```

---
## \#164 Posted by: Print3r Posted at: 2017-05-17T13:01:29.394Z Reads: 219

```
I haven't done much work with screens but found this: https://arduino.stackexchange.com/questions/17766/how-to-display-variables-on-0-96-oled-with-u8glib-library
```

---
## \#165 Posted by: lox897 Posted at: 2017-05-17T13:04:25.314Z Reads: 219

```
Sweet thanks! Looking forward to seeing some of this code. I am trying to learn as much about it as possible to add extra features to RG's code. Are you aware there is a V2 of U8Glib? Not much difference though I believe.
```

---
## \#166 Posted by: Print3r Posted at: 2017-05-17T13:07:47.551Z Reads: 215

```
Nope, didn't know there was a v2 - use google as your friend (he knows a lot :slight_smile:).
```

---
## \#167 Posted by: Sander Posted at: 2017-05-17T13:37:52.579Z Reads: 229

```
I am using Adafruit's library if you are wondering.. ;)
It is easier to use.

@Print3r the method I will use now will work pretty good! And the link to that Arduino needs a FTDI to program. its no USB interface unlike the leonardo.

Here is the right one:
http://www.ebay.co.uk/itm/Pro-Micro-ATmega32U4-5V-16MHz-Replace-ATmega328-Arduino-HOT-MC-/262855140223?hash=item3d3363237f:g:NIcAAOSwCU1Yv6Wk

The thing that is stupid this only cost like 2 gbp and the ATmega32U4 chip from digikey cost 2.7 gbps.
And the best thing is the board for 2 gbp comes with the bootloader. Its cheaper because of manufactering.

So I will order a bunch of those ;)
```

---
## \#168 Posted by: Print3r Posted at: 2017-05-17T13:50:15.189Z Reads: 217

```
Not needing an FTDI to program is nice (I have already got one but for an extra 60p not needing one is worth it). The board looks nicely made (not loads of flux everywhere like on some clones)! Economics of scale can be rather amusing sometimes ... pcb + chip + resistors + usb port + bootloaded chip is cheaper than the chip on its own ... guess I too will take the board then!
```

---
## \#169 Posted by: Sander Posted at: 2017-05-17T13:53:25.514Z Reads: 212

```
So the pcb from oshpark cost 2.5$, and the arduino pro micro atmega32u4 cost the 2.54$.
And I can use all the components from that board to my pcb so the total cost will be around 6-15$ depending on which oled and nrf24l01 type.
```

---
## \#170 Posted by: Print3r Posted at: 2017-05-17T13:57:33.180Z Reads: 217

```
Then manufacturing costs, shipping cost and listing cost (if on ebay/ amazon). So more like $20-25 for those buying it, depending on how many are ordered! But $6-15 is a good hardware price. I assume you have taken into accout that there will be an NRF, pcb, atmega under the skateboard as well as in the remote.
```

---
## \#171 Posted by: Sander Posted at: 2017-05-17T15:09:46.265Z Reads: 232

```
[quote="Print3r, post:170, topic:22055"]
I assume you have taken into accout that there will be an NRF, pcb, atmega under the skateboard as well as in the remote
[/quote]

For the price I was talking abour the remote only. I have done nothing yet with the board but it works to use the same pcb ;)
```

---
## \#172 Posted by: lox897 Posted at: 2017-05-17T20:06:17.223Z Reads: 237

```
Thanks guys! Good luck!
```

---
## \#173 Posted by: Sander Posted at: 2017-05-20T01:05:55.619Z Reads: 242

```
https://www.youtube.com/watch?v=uOZm8NNdKU4&feature=youtu.be

I kinda dont like the menu subrow things.
Leave suggestions pls.


Thanks to @rwxr for 3D printing the controller and shipping it to me!
```

---
## \#174 Posted by: Print3r Posted at: 2017-05-20T07:48:28.862Z Reads: 238

```
The controller looks great - thanks @rwxr for printing and shipping it to @Sander.  I assume on the home screen what is shown at the start is the duty cycle - are you thinking of adding the various other things from a previous picture? If you don't like the menu subrow thing, you could just narrow it down to the essentials e.g. brightness (click on the word brightness and a slider appears under brightness that you can scroll up and down, click again to confirm and slider disappears), lights (click on word lights and on, off button shows up beneath row 'lights' push up or down to scroll between them and then click to enter), efficiency mode (again on off - speed and power limiter tuned in the app)? Most of the settings functionality should be built into the app - there is more screen space and you shouldn't be changing it while riding!

I have nothing against the current settings, but they are quite small and I can't make out what the highlighted row says in the video. What do you think of the flip up screen and the screen being vertical - should have time the weekend after this one and the whole of the next week to work on a printable design if people would prefer that - here it seems like your fingers will obstruct the screen whilst riding? Despite my many suggestions, great work @Sander for making so much progress on the controller code!
```

---
## \#175 Posted by: Sander Posted at: 2017-05-20T11:02:13.651Z Reads: 226

```
Thanks!

Well I will find a way out to make it cooler, searching up subrows, etc :blush:

I think it should be possible to change the max speed and max acceleration on the app.
And on the controller you could do the same and if you dont want the "Custom" mode you can just change it to "Beginner", "Advanced" or "Experienced"

The finger will probably be in the way, but I hold the remote a bit different. So it will not be a issue for me.

I dont know if its possible to flip it vertically but I can try to make a new code for vertically screen later when I am done with this one :)
```

---
## \#176 Posted by: Print3r Posted at: 2017-05-20T13:32:23.886Z Reads: 234

```
Have fun making the display cooler - be inventive! I didn't really understand how you can change the screen colour in code - on the internet you seem to buy a blue oled screen or a white one?

You are right, I think changing the mode is very important. I will design the new controller next weekend for the bigger screen - you have set the design standard very high! Finish your setup first before working on the vertical version - it is very kind of you to do both though you will probs use yours!
```

---
## \#177 Posted by: Sander Posted at: 2017-05-20T13:38:48.261Z Reads: 257

```
You cant change the color on the display but you can buy a 16bit high resoulition display but it works much different. You create the menu/pages in an Editor where you commicate with the UART port with the oled display.
And ofcourse the OLED with colors are 10 times more expensive ;)

I have changed the menu again, I like it much better now.
https://www.youtube.com/watch?v=ZrKJcVGCksA&feature=youtu.be
```

---
## \#178 Posted by: Print3r Posted at: 2017-05-20T13:39:41.360Z Reads: 274

```
Like it much more now - looks much cleaner
```

---
## \#179 Posted by: Sander Posted at: 2017-05-20T13:41:12.198Z Reads: 274

```
Beside the OPTIONS on the top it will have the battery percents on left side? And the bluetooth symbol on the right if the phone is connected.

And on the home screen it will have the current time in the middle on top.

Time to work on the lights page...
```

---
## \#180 Posted by: Sander Posted at: 2017-05-20T15:29:17.879Z Reads: 282

```
I might start using uglib8 because of the memory is getting short. 
I will switch to it if it creates issues in the future.

On the home screen:
**Top left** is the distance you have droven total, **top middle** is the time. **top right** is the battery percent left of your board.
**Bottom left** is the amps, **bottom middle** is the potentiometer value(debugging for now), **bottom right** is the volts.

In the **middle of the middle** where the 20 number is. It is the current speed in km/h but you can change it in the settings to mph in the future..

https://www.youtube.com/watch?v=6IIsJf0uKns&feature=youtu.be
```

---
## \#181 Posted by: Okami Posted at: 2017-05-20T15:41:20.561Z Reads: 257

```
Nice work! A pleasure to see it is developing further :D
```

---
## \#182 Posted by: Print3r Posted at: 2017-05-20T15:54:09.452Z Reads: 246

```
Amazing work - the layout is super clear. I do still think the extra screen size would be good as at the start of the video if not in full screen, it is hard to read some numbers (but I suppose you don't need to see battery percentage and km left etc. whilst riding). Where were you thinking of putting the turn signals - on either side of the speed?
```

---
## \#183 Posted by: Sander Posted at: 2017-05-20T16:02:58.946Z Reads: 237

```
I have no problem reading any values.
I know other people will have because they need glasses or do not see very well small object.
The easy fix is using a bigger display or use your phone to change the settings.

When you have connected your phone to the bluetooth with a destination to go to.
It will automatically change the home page to destination page.
Then the speed becomes irrelevant so it gets smaller font and the turn signal will replace the big 20 number. 

Or I can move the speed/(meters to turn) to the very left and the turn signal will be on the right so your hand will only block a bit of the 20 number so you get the speed and the turn signals.
```

---
## \#184 Posted by: Print3r Posted at: 2017-05-20T16:08:22.214Z Reads: 226

```
I think moving the speed to the left is better as (though I have never eboarded yet - building my board next month or after september) I assume that when riding you lose a sense of speed after a while and could be going way faster than you would like to be going. Also, I don't know if you have tested visibility outside in the sun @Sander, but I think the sun will make the smaller numbers hard to see (though they are of course not as important as the big speed number)!
```

---
## \#185 Posted by: Sander Posted at: 2017-05-20T16:40:41.128Z Reads: 230

```
You will not have any problem seeing the screen in the sun.
It is OLED and it has a bright brightness.
And not much reflections.

I will try to create the same Menu thing in u8glib now..
```

---
## \#186 Posted by: Okami Posted at: 2017-05-20T16:43:03.080Z Reads: 232

```
yeh oled should be fine I think :) letters / numbers usually are quite fine. Havent tested on in sun but I do know it is hard as hell to see anything on LCD display in direct sun (unless leds illuminating the display are super bright)
```

---
## \#187 Posted by: Sander Posted at: 2017-05-20T16:57:24.512Z Reads: 224

```
Okey the U8glib is easier then the adafruit because this has almost auto text aligment.
Uses so much less RAM then the adafruit.
```

---
## \#188 Posted by: Print3r Posted at: 2017-05-20T16:58:33.877Z Reads: 219

```
You can further limit the memory usage by making the arduino store only the characters of each font that it will need.
```

---
## \#189 Posted by: Sander Posted at: 2017-05-20T16:59:24.742Z Reads: 224

```
Thats a smart idea.
For the speed I only need the numbers not the alphabet.

Btw I am recreating the menu right now in the U8glib.
```

---
## \#190 Posted by: Print3r Posted at: 2017-05-20T18:33:43.802Z Reads: 237

```
U8glib also means you can rotate text ... vertical screen? ;) 

e.g. from  http://henrysbench.capnfatz.com/henrys-bench/arduino-displays/oled-arduino-blue-1-3-sh1106-display-quick-start-tutorial/ 
void u8g_string(uint8_t a) {
  u8g.drawStr(30+a,31, " 0");
  u8g.drawStr90(30,31+a, " 90");
  u8g.drawStr180(30-a,31, " 180");
  u8g.drawStr270(30,31-a, " 270");
}

Had a thought for a feature that would be cool but hard to do: have on the iphone a grey pixel grid of the screen and allow people to design their own layout. Would be super difficult though and too many font sizes might be chosen so the processor wouldn't have enough space for it all.
```

---
## \#191 Posted by: Okami Posted at: 2017-05-20T18:41:22.436Z Reads: 229

```
crazy.. I saw all these animations for oled screen.. the functions and things you can make on it are just fantastic!..

Someone definately needs to integrate a display also in the deck to show cool info there :D
```

---
## \#192 Posted by: Sander Posted at: 2017-05-20T18:43:52.631Z Reads: 227

```
I know thats cool!

But I have a slightly problem...
On the Adafruit's library when the oled updated you couldnt see pixel for pixel row change it all went together.

With this library you can see it updates from top to bottom.
I am a bit too much perfectionist....
```

---
## \#193 Posted by: Print3r Posted at: 2017-05-20T19:13:32.693Z Reads: 225

```
This might help http://henrysbench.capnfatz.com/henrys-bench/u8glib-graphics-library-user-guide/u8glib-arduino-oled-tutorial-2-playing-with-the-picture-loop/! It is always best to have a perfectionist writing the code! @Okami The screen is quite small and the bigger ones are more expensive so having an oled showing stats and directions on the remote is better I think.
```

---
## \#194 Posted by: Okami Posted at: 2017-05-20T19:15:19.130Z Reads: 238

```
Well yeh I know, It was more meant for Single measurement displaying or maybe for battery status someone can also program up something neat..

Keep on doing the work on remote :D im just slowly realizing how cool these oled displays might be. Havent tried one yet..

I think @JTAG had one for his bms - battery and it also looked awesome
```

---
## \#195 Posted by: Print3r Posted at: 2017-05-20T19:18:59.946Z Reads: 249

```
Battery indicators can just use three seven segment displays and drivers or a row of leds - OLEDs look great but really push the arduino if all of the screen is used (really slow refresh rate) so I try to avoid them unless really necessary. But totally agree, animations are key if you have a screen - the splashscreen on startup has to have a super cool animation!
```

---
## \#196 Posted by: Okami Posted at: 2017-05-20T19:31:49.684Z Reads: 253

```
<img src="/uploads/db1493/original/3X/d/a/da4dc9d63adcc4e440e258d46ec209593969e3f9.png" width="666" height="500">

Or for example for this :D

Work of @JTAG

--

@Print3r How many lines of text can you fit in vertical way?

I think at least 8 you should.. that is just enough for 8s battery pack to see individual voltages.
Another way for 12s, it can be even made with 6lines but just in 2 columns..
```

---
## \#197 Posted by: Print3r Posted at: 2017-05-20T19:38:05.289Z Reads: 240

```
You can get almost any size of font imaginable ... yes you can fit all 8s/12s battery voltages on one screen, you just have to find enough analog inputs for each of the 8 or 12 cells and would have to build a voltage divider for each one (5V atmegas can only read voltages between 0-5V)!
```

---
## \#198 Posted by: Okami Posted at: 2017-05-20T19:40:14.046Z Reads: 255

```
Yeh, I think  voltage divider is not a problem.

I had an idea awhile ago about Lcd display battery meter, perhaps even energy analyzer (with current sensor) but these oled screens looks like work really nice and can accommodate / fit a lot of text in small space.

--

One more nice design / screen picture:

<img src="/uploads/db1493/original/3X/4/5/45195f9e5c8c4bfcc2ca0df952ad864602b0684b.png" width="666" height="500">

I hope @ Jtag does not mind I share his oled screen creations :D
```

---
## \#199 Posted by: DiegoTheWolf Posted at: 2017-05-20T19:53:43.601Z Reads: 252

```
Hey mates,

to be honest, i didn't read the whole thread.
BUT
I started making a simple Remote (With screen and throttle settings, menu, etc.) myself and got some code together.
Since i will switch jobs soon, i stopped all my DIY projects to get ready to move.

Maybe you can use anything of my (amateurish) code.

https://github.com/DiegoTheWolf/EMTB

Feel free to ask if you want more information.
If it doesn't help, just leave it ^^

Greetings
Diego
```

---
## \#200 Posted by: Print3r Posted at: 2017-05-20T19:57:20.285Z Reads: 239

```
The library you use for the screen seems very fast! Same here for time - I also don't have time to do any DIY projects for another couple of weeks!
```

---
## \#201 Posted by: DiegoTheWolf Posted at: 2017-05-20T19:59:13.889Z Reads: 243

```
The library is scary fast.
Modified it to have some more utility (text alignment).
Works great with an Arduino nano, even an 8MHz pro mini ^^
```

---
## \#202 Posted by: Sander Posted at: 2017-05-20T20:38:38.488Z Reads: 233

```

I will give it a try if I cant fix the refresh rate! ;)
The refresh rate on the adafruit library is super fast, but it takes so much space!
```

---
## \#203 Posted by: Fabian287 Posted at: 2017-05-20T21:00:28.762Z Reads: 232

```
Try to use SPI oled. They are way faster
```

---
## \#204 Posted by: Sander Posted at: 2017-05-20T21:01:50.423Z Reads: 240

```
It is I2C Oled.
Its only the U8glib library that is slow af.
On the videos above I used adafruits libraries.
You cant see the refresh rates.

But I think I fixed the refresh rate by moving all the voids before the setup and the loop so it gets intalized before getting displayed or something like that. or not....

The SPI is almost 4 times faster then the I2C.
```

---
## \#205 Posted by: Sander Posted at: 2017-05-20T22:51:56.550Z Reads: 251

```
[quote="lox897, post:163, topic:22055, full:true"]
How do you guys display variables with U8Glib?
[/quote]

I finally found it out. Took me a few hours to figure out how.
Its pretty hard to find when you dont know where to look.
Espically when the U8Glib doesn't tell you how to insert values.

So I found out to display integer value:

> const char *text= "";

> int a = 1;

>   char b[5]; //Should be good enough for 4 characters. -100 to 100. Increase [5] if you need higher numbers.

>   String str;
>   
>   str = String(a);
>   
>   str.toCharArray(b, 5); //Should be good enough for 4 characters. -100 to 100. Increase 5 if you need higher numbers.
>
> text = b;
>
> u8g.drawStr(0, 54, text);

And here is for the float 
> char result[8]; // Buffer big enough for 7-character float
> float value = 25.02;
>  dtostrf(value, 6, 2, result); // Leave room for too large numbers!
> text = result;
```

---
## \#206 Posted by: JTAG Posted at: 2017-05-21T10:07:07.681Z Reads: 225

```
Haha no worries! They are all either Google images or paint creations. It is easier to create logos than it is to printr text ( I am still to lazy to write code for that xD.
```

---
## \#207 Posted by: Sander Posted at: 2017-05-21T10:53:39.565Z Reads: 236

```
Well I will  have a current sensor on the board, rx side.
It will get powered on when you are charging your board so  you can see how much you have charged your board in mAh.
That allows you to see how much you have used and how much  you have charged.
So on the remote on the oled will show precisely how much mAh or percent is left of the battery ;)
```

---
## \#208 Posted by: Okami Posted at: 2017-05-21T13:47:31.143Z Reads: 233

```
@Sander  Very cool. Had missed it probably as i jumped in only at the end of this discussion.

I had something like this in mind also so if you create that, it would be nice!

Started too late into electronics I assume :D and not enough infrastructure around me to continue it on daily basis :\

So yeh, please when you finish it up, show it to others :D so that they can see what is possible and how cool it is. Otherwise bms charging is now like a black box, at times only thing you see is either red or green light lol.
```

---
## \#209 Posted by: ACIN Posted at: 2017-05-22T00:07:48.923Z Reads: 230

```
Yeah I would switch places with my board to own one of those remotes. Really into board lighting which this is perfect for.

 One day hopefully
```

---
## \#210 Posted by: Sander Posted at: 2017-05-22T05:42:44.988Z Reads: 243

```
That day is not very far from today!
Only 1 - 3 month left and the mold + the code should be ready, the receiver too.

Which LED's were you gonna use? Only one waiting for HIGH or LOW signal?
Because I will atleast add the feature for neopixel.
With the neopixel you can change every single light to whatever color.

So you choose which led configuration you have on your remote like: "Neopixel" or "Regular led".
```

---
## \#211 Posted by: ACIN Posted at: 2017-05-22T13:30:01.643Z Reads: 262

```
I very much look forward to that day!
I think the neopixel feature is definitely worth adding, although I am only using a standard (neutral white) monocolor LED Strip and I already have the 12V power supply that it runs on from my SBEC.
So for me personally I would just need a remote controlled inbuilt switch on the receiver or the "Regular LED" function.
```

---
## \#212 Posted by: laikiux Posted at: 2017-05-23T17:26:01.775Z Reads: 269

```
Mad Munkey Mod and Vesc telemetry :sunglasses:
<img src="/uploads/db1493/original/3X/c/1/c17380f026e6bb1ecd29c3c37442fc56c1ff9dc9.jpg" width="374" height="500">
```

---
## \#213 Posted by: keegancdr Posted at: 2017-05-23T19:53:04.387Z Reads: 257

```
woahhhhhhhh ?!?!
```

---
## \#214 Posted by: Fabian287 Posted at: 2017-05-24T12:22:15.682Z Reads: 262

```
<img src="/uploads/db1493/original/3X/5/4/547664fb847f05e735362de20a6d0d3c69ef3e8d.jpg" width="375" height="500">😇
```

---
## \#215 Posted by: keegancdr Posted at: 2017-05-24T15:48:31.083Z Reads: 255

```
but how?!?
```

---
## \#216 Posted by: Sander Posted at: 2017-05-24T17:26:00.692Z Reads: 264

```
I just receieved the smd long range. But I wont get to test them by next week because I am going to my cottage.

<img src="/uploads/db1493/original/3X/6/e/6e25306225da1cc42f8f2fcc6af2cf71f7de5b09.png" width="375" height="500">
```

---
## \#217 Posted by: Print3r Posted at: 2017-05-24T18:23:54.183Z Reads: 257

```
You bought 10?!
```

---
## \#218 Posted by: Sander Posted at: 2017-05-24T23:34:40.903Z Reads: 260

```
yeah ;P
.. . . . .
```

---
## \#219 Posted by: Sander Posted at: 2017-05-25T14:37:14.199Z Reads: 266

```
Well now it is almost the same menu in u8glib like it was in the adafruit. I will use a SPI Oled in the future because of the refresh rate. (Sorry for orientation)
https://youtu.be/94bOKdhtjz4
```

---
## \#220 Posted by: Sander Posted at: 2017-05-26T22:53:41.244Z Reads: 271

```
I don't know if many people are still watching this thread but here is a poll of how many that wants to buy it. 
Before you vote:
**CURRENTLY ONLY COMPATIBLE WITH IPHONE(Bluetooth)**

OLED Remote on the receiver side includes:

- Current Sensor (Reads ACCURATE Battery Percent/mAh)
- Bluetooth (Custom Remote Modes + Graph of ride tour + Turn by Turn Navigation)
- Lights Output

On the OLED Remote:

- 0.96" Display White
- Easy Menu to Use
- Turn by Turn Navigation System
- Shows current voltage, ampere, rpm, battery percent, local time, speed km/h-mph etc.
- Custom Acceleration speed
- Limit Max Speed
- Statistics
- Turn off and on lights, change color and blink mode.
- Create custom ride mode on iphone/remote.
- Total Distance droven(km/miles).
- Cruise Control.
- Over kill connection range(reliable remote).
- And more to come (please suggest)

I will make that you can update the remote at home.

The price is $59.9 // Cheaper then the Unreliable WINNING Remote

I do this poll to see how many I need to produce:
[poll max=1]
* Yes
* Maybe
* No
* Price is too high
[/poll]
```

---
## \#221 Posted by: Jinra Posted at: 2017-05-26T23:03:42.806Z Reads: 263

```
It's a remote and bluetooth module in one. $60 is fair IMO. Will definitely pick one up if I like the final design.
```

---
## \#222 Posted by: markyoe Posted at: 2017-05-27T04:16:53.703Z Reads: 263

```
If you ever develop it for Android, I'd definitely be interested.
```

---
## \#223 Posted by: Sander Posted at: 2017-05-27T10:18:24.345Z Reads: 264

```
Sure! But I have no android to do so. But if the develop program has a simulator I will do so.
```

---
## \#224 Posted by: rpn314 Posted at: 2017-05-31T00:10:55.620Z Reads: 260

```
Android Studio does have an emulator. I'd be happy to help with the android side if you'd like some help. I've done some android development, though I'm principally an iOS user myself.
```

---
## \#225 Posted by: rwxr Posted at: 2017-05-31T11:38:29.071Z Reads: 263

```
Have you guys seen this?
Faraday seem to be working on a thingy-dingy based on arduino. See section 2 in the blog.
http://www.faradaymotion.com/blog/

http://forum.faradaymotion.com/d/4-refactoring-the-faraday-motion-core-software/10
```

---
## \#226 Posted by: Sander Posted at: 2017-05-31T11:58:46.840Z Reads: 255

```
Sure! Do you know how to add the Google Map API for turn by turn navigation? Then you need to make it send via bluetooth.
The value for turn right in x meters are like this:
AR,10 (a right in 10 meter)
Same for left, straight.
I have not included the round about yet.

Turn,Xmeter
```

---
## \#227 Posted by: Print3r Posted at: 2017-05-31T12:39:15.598Z Reads: 280

```
Sure does look interesting but all I have seen on the ESP modules is bugs and faraday motion is not going to be selling theirs without a markup! It is nice to see that other 'big name' manufacturers are following a similar route though!
```

---
## \#228 Posted by: Sander Posted at: 2017-06-16T17:31:49.084Z Reads: 276

```
Doing some progress...

https://www.youtube.com/watch?v=ZbinadcS58w&feature=youtu.be

You can turn on and off the VESC, its because when the voltage is low, it will tell you,when you brake and the rpm is very small the VESC's will turn off automatically.

The Arduino is 24/7 on for now, in this version.
Its connected via the antispark, it has not fried yet, 2.3A tested.

The update of the Ampere may seem slow, because its average motor ampere.

You may ask why it is Color in the Power section on the OLED.
Its because the section is actually the Lights section.
I renamed it to Power from Lights because it was the only function section that are working.
```

---
## \#229 Posted by: NAF Posted at: 2017-07-05T17:03:28.938Z Reads: 250

```
Any progress? Can't really wait for this remote !
```

---
## \#230 Posted by: wafflejock Posted at: 2017-07-05T22:36:36.339Z Reads: 261

```
This thread needed to exist like a year earlier so I could have saved my time and money not duplicating work :) in all seriousness I didn't do any OLED integration although I do have one laying around so it's nice to see a project that has already been working a lot on integrating it into the remote and giving it useful functionality.

My simplified version of this is here https://github.com/shusain/eskatecontroller

http://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/1905

---

I'm just sending through the throttle signal though so lots of "missing features" though really I wanted to be sure the connection and programming was solid without needing to worry about extra data parsing and transmission.  Just got some PCBs made they are $2.80 a piece shipped if you get 10 (or $5.60 if you get 5 it doesn't matter the cost is shipping not making them).  Still need the hard candy shell but looks like there are at least a few iterations here.
```

---
## \#231 Posted by: wafflejock Posted at: 2017-07-05T22:43:57.972Z Reads: 244

```
I'm also curious if anyone knows the legal ramifications for selling a transmitter and receiver that hasn't been certified by the FCC or whoever handles that in the EU or elsewhere.  I thought about doing my own but the whole selling a built transmitter thing put me off (high fees to get certification and not enough audience to make it worthwhile to do a large scale production).

---

I know from Ada Fruit sites you can sell kits with FCC certified radios and the kit doesn't need to be certified and you can make prototypes (I think up to 5 of a given thing) without having to do anything but beyond that it gets murky what you have to do or cannot do.
```

---
## \#232 Posted by: Sander Posted at: 2017-07-05T23:04:49.958Z Reads: 228

```
Nice remote, the FCC thing I dont really know what to do with that. I guess I gotta sell them "unverified" and see what happens ;)
```

---
## \#233 Posted by: wafflejock Posted at: 2017-07-05T23:06:39.198Z Reads: 238

```
Yeah I think this will be under the radar enough (literally and metaphorically) to not matter much honestly just not sure what happens if you get "caught" or who is even checking?  Also I figured if I wanted to publicize and all it would be something I should check out before-hand, not saying you shouldn't do this you'll probably be fine but not a lawyer so take it with a grain of salt.
```

---
## \#234 Posted by: Sander Posted at: 2017-07-05T23:10:36.255Z Reads: 231

```
If I get caught immediately stop using the device, don't use it again, and you should be okay. I'll see if I can get a FCC license of the nrf are good. "Stick to the ISM bands (13.56MHz, 27.12MHz, 40.68MHz, 915MHz, 2.45GHz, and 5.8GHz, +/- a bit for each) for added comfort."
```

---
## \#235 Posted by: wafflejock Posted at: 2017-07-05T23:15:15.675Z Reads: 228

```
I just wonder if aside from cease and desist order if there is a major financial penalty that makes it not worth what probably will amount to a few hundred to low thousands of dollars (if the risk is a $10,000 fine I wouldn't personally do it without the certification since that costs like $10,000 from what I've read).  There's also self certification for FCC too though so like I said need someone who knows the law and technical details.
```

---
## \#236 Posted by: Sander Posted at: 2017-07-05T23:15:34.256Z Reads: 234

```
Well it seems there are a different version of the nrf24l01 module that is FCC verified. I only need to ask for the FCC id and pay for the fcc testing. And I gotta get the IC FCC verified too. I think this will be fine :)
```

---
## \#237 Posted by: wafflejock Posted at: 2017-07-05T23:17:32.082Z Reads: 228

```
Yeah I was thinking also you could sell it as a "kit" I wonder how many components the end user has to connect to make it a "kit"
```

---
## \#238 Posted by: Sander Posted at: 2017-07-05T23:20:58.556Z Reads: 224

```
Hmm, if I have all the smd components soldered and I have the oled, buttons and the potentiometer not soldered. Like you solder them yourself?
```

---
## \#239 Posted by: wafflejock Posted at: 2017-07-05T23:21:45.728Z Reads: 236

```
Yeah really not sure if that counts or not like I said read up on it a bit on adafruit and a few other places but couldn't find clear answers... you'll probably be fine but worth checking out for an afternoon at least.
```

---
## \#240 Posted by: Sander Posted at: 2017-07-05T23:24:27.137Z Reads: 246

```
Nothing much... Have been on holiday and not quite motivated because a guy named Alextech on this forum I bought from (Dual Hub Motor, Custom 12S4P Battery) has never arrived to me, been shipped once and never again, when it was in Norway it got returned and he didn't ship it again, he said he will send me the hubs but he went silent again... Spent around $440 on it. 

Thats why I dont have done alot of progress because I have nothing to keep me motivated. If I had those I would work on my remote non stop beause I want to ride the board. I have waited over 130 days for the parts.
```

---
## \#241 Posted by: wafflejock Posted at: 2017-07-05T23:25:44.715Z Reads: 245

```
That sucks saw the alextech thread sorry to hear you've been without parts because of it, that really sucks.  Hopefully he can set things straight.
```

---
## \#242 Posted by: ACIN Posted at: 2017-07-05T23:31:33.904Z Reads: 236

```
I pray to the Esk8 Jesus you will get your hubs soon :disappointed_relieved:
```

---
## \#243 Posted by: Sander Posted at: 2017-07-05T23:36:40.781Z Reads: 248

```
[quote="wafflejock, post:241, topic:22055"]
alextech thread
[/quote]


Can you give me the link to the thread, thanks.
[quote="ACIN, post:242, topic:22055"]
I pray to the Esk8 Jesus you will get your hubs soon :disappointed_relieved:
[/quote]

Thanks alot, I have waited so long for these items and now I feel the items doesnt exist.
```

---
## \#244 Posted by: wafflejock Posted at: 2017-07-05T23:39:25.638Z Reads: 251

```
http://www.electric-skateboard.builders/t/horrible-communication-by-alextech/25597/56
```

---
## \#245 Posted by: Sander Posted at: 2017-07-06T00:46:01.968Z Reads: 255

```
Well here is my story:
http://www.electric-skateboard.builders/t/horrible-communication-by-alextech/25597/69

And I actually paid him $685 for him to waste my time for 6 fully months.
```

---
## \#246 Posted by: wafflejock Posted at: 2017-07-06T02:52:34.144Z Reads: 251

```
Sorry to hear it but glad you got to post your experience too.  I bought my motor and batteries from hobby king and got the rest of my components from  just wanted to put it out there that not all the small vendors like diy have such problems typically.  (Usually items are in shipping within a day or two of the order and they just updated the site some to make viewing old orders easier)

---

That said make sure you don't fall into the traps of not knowing shipping or customs fees that will need to be covered for any physical good and lead times for components and possibly getting bad batches that need to be replaced these are realities for anyone trying to ship any physical goods.
```

---
## \#247 Posted by: NAF Posted at: 2017-07-06T06:37:42.246Z Reads: 247

```
That's a real bummer and I am sure that you will get your money eventually back from him after Paypal disputes.....but to be honest dude...this remote is really amazing and you could organize a group buy here and make many times over on this remote than what you lost on Alex. I am pretty sure there will be tons of buyers here for this remote...and there is nothing more motivating than a stream of money that you can later spend on ESK8 :) :slight_smile:  There you go ...that's your motivation :slight_smile:
```

---
## \#248 Posted by: wafflejock Posted at: 2017-07-06T06:42:21.080Z Reads: 252

```
Agree this looks like a lot of well done work so far and most of the controllers seem to be pretty flakey at best and dangerous at worst.  Haven't checked out your code yet and I had some patches to my own due to failures while operating but would just make sure you CYA and make sure you understand all your costs risks time for assembly and shipping.  Taking orders isn't something you should rush into.
```

---
## \#249 Posted by: Sander Posted at: 2017-07-06T10:23:59.811Z Reads: 263

```
@NAF Thanks

@wafflejock I know, ;)
```

---
## \#250 Posted by: Sander Posted at: 2017-07-07T21:48:28.457Z Reads: 269

```
I will create these for my Reciever atleast. Because I dont have space inside the receiver layout. 
But if I make an "addon" on it I have no problem with the space ;)

So I have come up with this little guy. It has an antenna and I hope the signal will be steady :slight_smile: 
Should be better with that antenna then the inbuilt copper antenna.
<img src="/uploads/db1493/original/3X/c/b/cbd3890ccb1c2b9be7521f44f9a641a0b82ac039.jpg" width="520" height="500">

This image should appear as the realsize on a desktop:
<img src="/uploads/db1493/original/3X/7/d/7d4e74e86fbe687333059bc3b90636b96b6247dc.jpg" width="28" height="34">
```

---
## \#251 Posted by: wafflejock Posted at: 2017-07-08T15:38:14.884Z Reads: 265

```
This would be nice in terms of general purpose can get it surface mounted and all but I'm kinda curious why not just put an Atmel chip or other MCU right on here as well.  When I made my PCB I was just doing something to get rid of the wire clutter, but if you're going to get one with assembly as well think you might as well just go the extra couple of steps to put the mcu right on here with the radio.  This way would just be one PCB, all you need from say an ATMEGA328P is the 7 lines to the NRF chip and going into it just needs regulated 3.3V (it has an internal oscillator that will run the chip at 8MHz if you don't have an external one).  For reading the potentiometer (controller trigger) just need one of the analog pins from the MCU and for writing PWM just need one of the PWM capable digital pins (receiver to ESC).

---

Extra note, would need to be sure to break out the pins for programming the Atmel chips as well, still it is probably worth it if you're going to have the fab house do assembly.

---

Also not sure if you've seen them already or not but there is an ESP8266 (I'm pretty sure is the model) that has wifi and can be reprogrammed but I haven't really checked out doing ad-hoc type radio to radio communication with them (don't have one just seen videos) they might be worth checking out before going the route of custom assembled PCBs.  Regarding the built in antennae it has worked fine for me so far but for whatever reason I would feel more comfortable with a real wire coil antennae.
```

---
## \#252 Posted by: Sander Posted at: 2017-07-08T18:14:29.522Z Reads: 240

```
Well I dont kinda like the ESP8266, it crashes alot, one reason is I use OTA.
But I love the range with them. Right now I dont gonna do much because I have ordered the receiver pcb etc.
```

---
## \#253 Posted by: Sander Posted at: 2017-07-30T22:56:59.390Z Reads: 241

```
No, I am not giving up, the signal is terrible and the nrf lacks many features. 
I will be moving on to another transceiver that has good range, encryption and private network.
It even has a RSSI feature. (Receive Signal Strength Indicator). It’s a measurement of how strong the transmission was when a message was received. So I can create a little signal test icon for debugging.

The radio is even license free.
```

---
## \#254 Posted by: Ackmaniac Posted at: 2017-07-30T23:04:20.963Z Reads: 233

```
Sounds like you want to go WiFi with ESP8266 or ESP32.
```

---
## \#255 Posted by: Sander Posted at: 2017-07-31T00:10:40.848Z Reads: 231

```
Generally dont like to use those because you send data and receive with using client.println (basically serial) etc, which is not fast enough for getting values from vesc, send to controller and send back to vesc. If there is any way to send packages to each other like on the NRF (which may be possible) I will give it a try again.
```

---
## \#256 Posted by: Ackmaniac Posted at: 2017-07-31T06:40:02.478Z Reads: 242

```
There is also a write function. But the connection reliability isn't that great in crowded environments.
```

---
## \#257 Posted by: Sander Posted at: 2017-07-31T10:38:03.294Z Reads: 251

```
Yeah, it will be a lot of disturbed I guess? Its a WiFi module, there are alot of wifi's around. 
Thats why I go for a low frequency license free radio ;)
```

---
## \#258 Posted by: jess.t.moody Posted at: 2017-08-06T05:35:54.712Z Reads: 254

```
I'm looking to incorporate a WS2812 RGB LED strip on the rim of my board. I was just planning on connecting an Arduino to them, but it would be awesome to be able to control them from the remote. Any way you could add LED strip control functionality? Thanks! Looking great so far! Keep it up!
```

---
## \#259 Posted by: Sander Posted at: 2017-08-06T12:08:11.952Z Reads: 247

```
Sure? But I have that u can controll adafruits neopixels, they might be the same version.
```

---
## \#260 Posted by: jess.t.moody Posted at: 2017-08-06T17:33:59.847Z Reads: 242

```
I think I saw the video with the LED changing color, but I didn't realize that was a WS2812 (Neopixel). Awesome! Would you be able to do patterns as well?
```

---
## \#261 Posted by: Sander Posted at: 2017-08-06T19:00:50.984Z Reads: 238

```
They are WS2812B or SK6812-based LEDs (Same protocol etc).
On my first build I had blinking, fading, strobe, breathing mode for the leds, controlled via iPhone.
So yes, and you will be able to create pattern too.
```

---
## \#262 Posted by: Sander Posted at: 2017-08-15T00:58:22.047Z Reads: 238

```
Ok, I have been testing with bluetooth to bluetooth(HC-06).
It is super fast and the code I wrote is pretty solid. The range is amazing! Through 3 floors down(3m heigh) with doors closed. 

I have managed it to send potentiometer value and receive the voltage, amps etc. So far its working good. 

But this version I am using bytes because the .write function is a uint8_t that I believe is 8bit so the maximum number/bit is 255.

I might give the ESP8266 MCU a try, because the same code will work for that.
```

---
## \#263 Posted by: ACIN Posted at: 2017-08-21T22:19:20.943Z Reads: 236

```
>But this version I am using bytes because the .write function is a uint8_t that I believe is 8bit so the maximum number/bit is 255.

>I might give the ESP8266 MCU a try, because the same code will work for that.

Uhuh my thoughts exactly :sweat_smile:
I wish you great fortune in the wars to come so I can one day finally throw my money at your face!
```

---
## \#264 Posted by: GCB Posted at: 2017-08-26T19:16:38.205Z Reads: 234

```
So when these go to market are you only selling a limited amount? Not gonna lie I'm really interested with this thread lol
```

---
## \#265 Posted by: Sander Posted at: 2017-08-28T20:13:51.913Z Reads: 223

```
Yeah I will sell some ;)
```

---
## \#266 Posted by: GCB Posted at: 2017-08-28T22:38:22.145Z Reads: 228

```
How much are you gonna sell them for? (If you do you should totally save me a spot because I will pay for one ;) )
```

---
## \#267 Posted by: banjaxxed Posted at: 2017-08-28T23:15:40.939Z Reads: 232

```
I'm also interested depending on cost dude
```

---
## \#268 Posted by: GrecoMan Posted at: 2017-08-28T23:16:58.289Z Reads: 231

```
I would be down to buy one depending on cost also
```

---
## \#269 Posted by: MorrisHsu Posted at: 2017-08-29T03:55:15.989Z Reads: 229

```
Looks cool I'm looking forward to your results I really want to buy one
```

---
## \#270 Posted by: Sander Posted at: 2017-08-29T05:59:01.389Z Reads: 233

```
@banjaxxed and @GrecoMan the cost will be depending on what you choose like. Current sensor and Switch with the receiver so you can turn off and on the board by powering the remote. With the current sensor get accurate reading of how much battery capacity you have left, and it estimates how far you can drive with it.
```

---
## \#271 Posted by: driver Posted at: 2017-08-29T08:55:37.913Z Reads: 232

```
How much ist the complete package?

So you have Photos in how ist will Look Like?
```

---
## \#272 Posted by: banjaxxed Posted at: 2017-08-29T10:19:49.287Z Reads: 234

```
Great work by another electronics guru BTW! Thanks for your contribution to the community.

Interested in the complete package, the whole shebang. Was also looking at Wajdi's one but far too expensive IMO, hoping this is less costly, maybe I'm not realistic about the effort and cost that goes into building them. I may need to wait for mass-market adoption.
```

---
## \#273 Posted by: wafflejock Posted at: 2017-08-29T20:47:34.968Z Reads: 243

```
I think this is pretty accurate:

https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit#gid=0

I looked at making my own into a thing to sell for people but got super paranoid about all the regulations around selling things with radiators.  After talking with a friend who does product development he told me basically any circuit that has a potential oscillator/loop in it basically has to go through certification before they can actually produce it.  The certification process isn't impossible but it is costly so the only way to recoup the cost is to sell them at a pretty large scale which makes this a somewhat risky endeavor given our community isn't absolutely everybody :)

I still made my own.  The radios were $2 a piece but I bought 10 and the arduino pro mini 3.3V I used for mine were also around $2 a piece and I got 5 (only need 2 of each but good to have spares).  The PCB I made for my own version of this cost $28 to get 10 of them shipped, any lower quantity still cost $28, because of shipping.  Aside from those components need at a bare minimum a potentiometer or a hall effect sensor and a battery (I used a 800 mAh).

---

Basically this is a good deal if everyone is building their own and people buy in groups of 5 at least and split components from sets of 10 then you can get decent prices on everything and not have lots of spares.
```

---
## \#274 Posted by: GCB Posted at: 2017-08-30T02:53:25.231Z Reads: 222

```
Saber would it be possible to make a setting to translate km to miles? Also did you make a functional version yet?
```

---
## \#275 Posted by: Sander Posted at: 2017-08-30T21:37:02.361Z Reads: 234

```
Yes its possible and what I had in my mind ;) 
Yes it is functional too! But with the menu I haven't done yet because I needed to create a strong foundation first for it, so it doesn't crash with no reason ;)

Right now it display's how much battery mAh you use, how many km you have left, battery percentage left, ampere, voltage, current speed(km/h) :)

aaaand I am experimenting with bluetooth because it auto connects to each others so other can't interfere I hope.
```

---
## \#276 Posted by: ossieeskar Posted at: 2017-09-08T01:06:15.932Z Reads: 235

```
Hey guys, this all looks crazy cool! Im in the process of building my first board and would like to try to build one of these as well or buy one. 
1) What does my board need to take full advantage of this remote? I have a dual hub motor 1800w 75kv, dual vesc, 12s2p 18650 battery. Do I need a bms to take full advantage? if so which one do you recomend that is reliable? Do I need a hm-10 in my vesc or just the remote? would I need the hm-10 on 1 or both of my vesc?

2) Will this be open sourced for us to try to build this remote for ourselves? any timeline?
```

---
## \#277 Posted by: Sander Posted at: 2017-09-08T16:03:28.858Z Reads: 245

```
[quote="ossieeskar, post:276, topic:22055"]
1) What does my board need to take full advantage of this remote?
[/quote]

Well, if you want to unlock your board to the full potential you use the remote I am making. With that I mean you can see precisely how much mAh left. Change the settings on the VESC with the remote. Different speed curves. Braking lights.
Get data of the ride on the board displayed on interactive graph on the phone.

With the hm-10 you are talking about, with this remote you will receive two things, a remote and a receiver with current sensor and electric switch on.

[quote="ossieeskar, post:276, topic:22055"]
2) Will this be open sourced for us to try to build this remote for ourselves? any timeline?
[/quote]

Yes I will probably open source it if I don't wanna produce some self. But I will atleast make 3.
```

---
## \#278 Posted by: ossieeskar Posted at: 2017-09-08T18:12:19.654Z Reads: 237

```
Awesome! thanks so much for getting back to me. 
Any idea how much and when they will be available? is there a waitlist? dibs on 1/3?? lol
```

---
## \#279 Posted by: Sander Posted at: 2017-09-09T18:34:44.878Z Reads: 234

```
All I can say right now is less then 60$.
I will be finished with this in 3 months I hope, if I can make a good schedule for more developing etc.
```

---
## \#280 Posted by: GCB Posted at: 2017-09-09T19:28:00.030Z Reads: 245

```
Nicee, my remote broke and I'm procrastinating on buying a new one because of price and reliability. If you have them in stock I'll try to buy one
```

---
## \#281 Posted by: ossieeskar Posted at: 2017-09-11T02:26:49.228Z Reads: 239

```
Yea definitely put me down! This remote sounds really amazing!
```

---
## \#282 Posted by: Sander Posted at: 2017-09-12T19:38:24.247Z Reads: 237

```
It will be a long time when I have them available, right now I am experimenting with momentary button to turn on and off the whole power in the board.
```

---
## \#283 Posted by: Sander Posted at: 2017-09-16T21:34:43.050Z Reads: 250

```
**Quick Update:**
Im going to give ESP to ESP a go. Because I have managed something very unique with them.
```

---
## \#284 Posted by: Sander Posted at: 2017-10-21T20:10:08.417Z Reads: 243

```
I am finally finished with my E-Board. So now I will order a few circuits to have on the desktop for faster developing of the remote ;)
```

---
## \#285 Posted by: monter_man Posted at: 2017-11-02T05:36:43.030Z Reads: 231

```
Hi Sander, are you in the US?  I have a couple of hub motors that I can contribute to your development, in exchange for help in my own build. If not, then I can donate $.     I'm using Adafruit bluefruit (M0 chip) and nrf24l01.  Could you pm, so we can discuss ?
```

---
## \#287 Posted by: GCB Posted at: 2017-12-24T01:22:00.745Z Reads: 209

```
You still working on these?
```

---
## \#288 Posted by: Texasguy Posted at: 2018-04-03T15:02:32.069Z Reads: 183

```
Any updates? This is an awesome idea, and would be really useful! More power to you!
```

---
## \#289 Posted by: Sander Posted at: 2018-04-08T22:01:28.328Z Reads: 178

```
Yes, I am now using other radio modules. The one I am using is amazing, the package is encrypted, the signal is very strong. From a room with door closed to a wall 15 meters away no signal change. It is documented that 150 meters should be no problem. With this one I can display the signal strength in dBm. So to the weekend I will have a working remote, but with the oled, connection to vesc will take some time. I am starting from scratch to make it solid ;)
```

---
## \#290 Posted by: Texasguy Posted at: 2018-04-19T17:56:22.384Z Reads: 161

```
I can't wait to see it in action! If you need any one to demo it, I think I could make that happen. :smiley: That  is so awesome to hear, I was worried that this project lost momentum and was bummed because it is such an AWESOME idea and development. Let me know if there are any ways I can help. I am not familiar with the electronic side of the remote operations (Mechanical Engineer), but I have a bunch of Electrical Engineer buddies at school that likely wouldn't mind lending a helping hand.
```

---
## \#291 Posted by: scorched Posted at: 2018-11-02T22:21:29.127Z Reads: 124

```
Is this remote still being worked on? I've been working on my own board slowly and j haven't found any remote that really impressed me except for the diy ones. I am absolutely terrified of the remote losing connection and I keep reading story after story about the go to remotes used on diy boards. Thanks in advance for any replies!
```

---
## \#292 Posted by: Sander Posted at: 2018-11-03T11:01:58.290Z Reads: 125

```
Yeah I am still working on it, its going slow because my board is made out of carbon fibre that kills the range + school. I have a demo working though, but it is not what I want, I want it to be super responsive and good range. To acheive that I need to filter to use low power noise amplifier and filter more the power.

My problem is finding a suitable radio to use. Right now I am using one with 16-bit encryption, so if another have the same controller it will not interrupt you, if I use nrf24l01 there are only pipes I can change and it gets more and more common. What I need is an auto-binding(like bluetooth), that feature I can make self but what is the chance for other to have the same id?

I got it working super good with 2 STM32, but I faced many issues. First was the update rate of the oled, then using oled and the radio did not work. Got that finally working. When getting details from the vesc, then the STM32 just crashes etc.

https://www.youtube.com/watch?v=NsXDMw_FnR4
```

---
## \#293 Posted by: StefanMe Posted at: 2018-11-03T14:55:58.932Z Reads: 116

```
Crazy so may remotes are in the line... what is the refresh time from the display? Just as a comparison for other diy remotes... in normal cycle with some values like speed, battery ect...?

looks nice!
```

---
## \#294 Posted by: Sander Posted at: 2018-11-04T13:19:07.476Z Reads: 102

```
Thanks, I have currently set it to 0.05 second. 
20 FPS. You don't need it to go any faster, only when you need animation.
```

---
## \#295 Posted by: StefanMe Posted at: 2018-11-04T13:50:48.193Z Reads: 96

```
No I mean how long do u need to refresh... not how often. Drawing including writing buffer or next page...
```

---
## \#296 Posted by: Zzazivsmazzi Posted at: 2019-06-11T07:32:47.943Z Reads: 53

```
Hi dear friend   i love this project         

Link   
 Not working 

Please   new uploading 

Please        thanks  for writing project
```

---
## \#297 Posted by: Zzazivsmazzi Posted at: 2019-09-11T10:23:02.905Z Reads: 26

```
Link not found    for download
```

---
