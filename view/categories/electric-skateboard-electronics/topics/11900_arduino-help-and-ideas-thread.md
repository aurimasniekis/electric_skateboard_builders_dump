# ARDUINO - help and ideas thread

### Replies: 152 Views: 8703

## \#1 Posted by: smudgeUK Posted at: 2016-10-25T21:34:53.503Z Reads: 466

```
I thought with the arduino projects a few people have ongoing we could have a social area to just talk about arduino. If people are having problems with code or wiring certain things up maybe we could discuss it here, hopefully it will keep peoples specific project threads clean and on track. I know im going to have various questions.
So far i know @EssEnn and @chinzw are currently working on things
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-25T21:36:53.091Z Reads: 430

```
Ask away! :slight_smile:
```

---
## \#3 Posted by: lox897 Posted at: 2016-10-25T21:37:01.763Z Reads: 423

```
Don't need any help with anything but just wanted to share this thing that I am making: 
http://www.instructables.com/id/DIY-Arduino-Battery-Spot-Welder/
I am using IRF1324, TVS Diode, and Schottky diode as an upgrade so the MOSFETS dont blow.
```

---
## \#4 Posted by: smudgeUK Posted at: 2016-10-25T21:39:49.706Z Reads: 420

```
noooo its absolutely fine @lox897 ... the more the merrier! Maybe you can assist us if we have questions ;-)
I may need a spot welder in the near future (2nd build !!) so il definately use that link as reference.
thanks
```

---
## \#5 Posted by: lox897 Posted at: 2016-10-25T21:45:40.568Z Reads: 401

```
I also know that Daniel from Melbourne ESK8 group has made leds that correspond to the amount of voltage the battery has.
```

---
## \#6 Posted by: saul Posted at: 2016-10-25T22:12:52.717Z Reads: 386

```
I've done this for my remote, with an atiny85.

Also working on brake/turn/under glow leds that plug into the rx ch1/ch2 and splits ch2 to esc.
```

---
## \#7 Posted by: Okami Posted at: 2016-10-25T22:20:46.008Z Reads: 375

```
I like the idea.. I think there shoud be a whole new category - ''arduino tinkering'' AKA ''arduino projects''

So far I've witnessed these applications for an arduino:

Battery level indicator (with simple leds)
Remote control ideas, using arduino
Data sending / receiving (speed, battery, ah/wh consumed etc)
Light control (headlights, turn signals etc)
Sound control.. (horn or similar)

Perhaps a few more..
```

---
## \#8 Posted by: saul Posted at: 2016-10-25T22:26:20.658Z Reads: 356

```
how about a uart to microsd data logger for vesc.
or even better a microsd config.xml to vesc uart programmer! :heart_eyes:
```

---
## \#9 Posted by: Okami Posted at: 2016-10-25T22:27:39.003Z Reads: 361

```
This would be great. IT could later be transferred to our ESK8 Database site using some sort of protocol and display the data there.. 

Btw, the current version is here, would be great to start collecting some direct data from Vesc's :slight_smile:

www.ej.uz/e8base
```

---
## \#10 Posted by: smudgeUK Posted at: 2016-10-25T22:35:56.760Z Reads: 350

```
I think as a group we could come up with a 'standard' reasonably straight forward setup which can be plugged in to vesc and, as you say, log certain parameters which would be useful for the database. 
Unfortunately im well out of my depth with logging info onto SD using arduino :-) but im more than willing to learn and follow along by building an actual logger.
Hell, it could be like 'today in arduino class' !
```

---
## \#11 Posted by: saul Posted at: 2016-10-25T23:13:13.184Z Reads: 332

```
well Arduino somewhat lead me to esk8....so its only right esk8 brings people back around.
```

---
## \#12 Posted by: chinzw Posted at: 2016-10-25T23:47:27.010Z Reads: 316

```
It should be pretty simple to implement this using rollingecko library. Once im done with the battery monitor ill use 2 of my free i/o to setup a serial to the vesc. That way i can get cells voltages and vesc data all to one chip.
```

---
## \#13 Posted by: smudgeUK Posted at: 2016-10-26T00:18:52.288Z Reads: 317

```
So @chinzw what should i be ordering to make a logger?
Is it as simple a list as:
-Nano 
-microsd card module
-cable and connector (which connector?) to go to the vesc
?

Ive got a few spare nano's, will order an sdcard reader and cable/plug once i know which size/type of plug is needed to plug into vesc
```

---
## \#14 Posted by: saul Posted at: 2016-10-26T00:23:48.747Z Reads: 304

```
lol I was just spitballin, I think it might be better with bt and just record on a phone. I just got a ble module to play with on android.

But if you want built in, a spi sd port like https://www.adafruit.com/product/254
and vesc uses 2.0mm pitch jst ph
http://www.ebay.com/itm/JST-2-0mm-PH-6-Pin-Connector-with-Wire-x-10-Sets-/171361716283?hash=item27e5f4483b:g:q3IAAMXQhpdRx6JR
```

---
## \#15 Posted by: smudgeUK Posted at: 2016-10-26T00:25:12.614Z Reads: 296

```
Or at least, a sub-category for arduino under 'electronics' ... i guess that all depends on how the forum is all setup but for now a thread should be fine.
```

---
## \#16 Posted by: chinzw Posted at: 2016-10-26T00:26:08.560Z Reads: 291

```
Setting up SD card is a little bit more complex, but there's plenty tutorials. If you buy the SD card breakout and RTC breakout you can just hook them up and they should work just fine.
```

---
## \#17 Posted by: smudgeUK Posted at: 2016-10-26T00:28:43.037Z Reads: 293

```
Ok cheers for that. I'll get a few ordered now along with an sd card module. Love the fact arduino modules and sensors are generally only a few quid.
i guess if the data is logged onto sd card and is easy to import into excel, a few variables like motor current and motor temperature (externally logged, not via vesc) could easily be overlaid on a graph to compare the heat influence certain current has on the motors.
Is there some sort of load calculation that can be done using current draw and rpm?
```

---
## \#18 Posted by: smudgeUK Posted at: 2016-10-26T00:29:32.459Z Reads: 282

```
spot on, thanks !
```

---
## \#19 Posted by: saul Posted at: 2016-10-26T00:35:04.439Z Reads: 282

```
yupp but they do add up :money_mouth:

if you're really going for it, I've always wanted to add a 10axis imu, so you can map hills, carves, direction...g force!

excel or csv to excel would be perfect, and then template some graphs.
I think current/rpm would be related to efficiency, lots of maths that can be done once some data is there.
```

---
## \#20 Posted by: smudgeUK Posted at: 2016-10-26T00:38:20.702Z Reads: 279

```
Ive already got an accelerometer/gyro module but when i looked at a few tutorials the code gave me a headache so i fell back onto the SOS led flashing haha
```

---
## \#21 Posted by: saul Posted at: 2016-10-26T00:43:55.240Z Reads: 255

```
true they usually give raw data.... still tho would be full data logger with that.
```

---
## \#22 Posted by: smudgeUK Posted at: 2016-10-26T00:50:09.543Z Reads: 250

```
This is true, its so easy to forget how much you've spent ... at least im nearly set up to log data long after the world has ended!
I usually sell something i no longer want/use on ebay and the money i have transferred to my paypal is my project spending money
```

---
## \#23 Posted by: saul Posted at: 2016-10-26T01:08:37.544Z Reads: 245

```
thats a good system to keep things going, I just throw it in a box for "later"
```

---
## \#24 Posted by: brandon Posted at: 2016-10-26T03:00:37.363Z Reads: 245

```
I'm designing controller boards to fit inside cheap chinese wii nunchucks so look forward to that in the future!
```

---
## \#25 Posted by: Okami Posted at: 2016-10-26T08:52:39.120Z Reads: 244

```
I think one of users on this forum already made a module called ''vesc bluetooth module'' he even created an app for iphone's and the app, I believe, was able to show graphs / charts, too! 

Perhaps there can be some cooperation made on how to make this to be recorded onto sd card..
```

---
## \#26 Posted by: Pimousse Posted at: 2016-10-26T09:15:51.777Z Reads: 251

```
Really nice thread !

I played a lot with Arduino and VESC.
I got working an "embedded computer" with
- Lights ON/OFF
- Brakelight
- Datalogging on microSD
- LCD screen with button for menu interaction
- Odometer

For that, I had to improve a bit the Rollinggecko's library to add fault management and temperatures.

Here is an overview of the project :
https://www.youtube.com/watch?v=IEq4MzafLBA 

However, I2C LCD, VESC comm, SD librairies, that was too much for my nano..
But everything was working separately..

Using the VESC UART with a HC05 now, I tried to measure directly battery voltage with a voltage divider. Worked well on the breadboard but my final solder on the prototype wasn't clean enough and I fried all (Nano + LCD) :smile: 

@chinzw  I'm not sure we could simply implement xml configuration loading though UART because of packet length.
MC_CONF command is a huge amount of data. It didn't matter for Vedder as far as he used USB connection.
But that's not impossible !
```

---
## \#28 Posted by: smudgeUK Posted at: 2016-10-26T09:48:59.248Z Reads: 229

```
I'm not sure what I'm looking at here ... :-)
@Okami, what would be the bare minimum we should look at trying to log for the database? If we cut all the un-necessary parts off the logger (no displays etc) so it is simply recording the minimum, I guess it would also be possible to reduce the amount of data by only taking a 'log' every second rather than 1/10th of a second (or whatever the sample rate would normally be)
```

---
## \#29 Posted by: smudgeUK Posted at: 2016-10-26T09:53:33.492Z Reads: 228

```
@Pimousse the magic smoke is never a welcome sight. I guess it went up quite nicely ;-)
Would you be interested in assisting with this little project seeing as you have basically already done it? As we mentioned above the goal would be to log some basic info to an SD card to collect data for the database. If you don't mind sharing your modified code with us I'm sure that would be a great start !
```

---
## \#30 Posted by: Pimousse Posted at: 2016-10-26T10:03:14.229Z Reads: 228

```
I'm so in love with open source and collaborative projects.
So I'll be so pleased to share everything.

I had datalogger working

http://img4.hostingpics.net/pics/729214IMG20160818131238.jpg

Here with random values.
I wasn't able to have I2C LCD, SD breakboard and VESC comm working simultaneously.
(I didn't find out why).

Honestly, I switched to the HC05 bluetooth module with VESC Monitor app for datalogging which is quiet more convenient.
So I didn't push the dev so far.
```

---
## \#31 Posted by: smudgeUK Posted at: 2016-10-26T10:32:03.360Z Reads: 219

```
Brilliant, thanks so much!
Would you be able to email it to me when you have a spare minute please, no rush at all - just when it is convenient for you!
I'll pm you my email address if this is ok :-) then i dont mind forwarding it to whoever else would like it.
```

---
## \#32 Posted by: EssEnn Posted at: 2016-10-26T12:49:10.566Z Reads: 211

```
@smudgeUK god I've had a lot of mentions in this thread. Sorry for the delay joining in, work has been intense. 

My plan for the Arduino is to control the PWM signal so you can adjust top speed and apply a delayed throttle curve to the ESC. This will make some boards easier to ride and when friends want to ride you can limit the performance so they won't get thrown off the board. 

So far I can read the PWM signal from the receiver, apply some smoothing to the result (average over 10 inputs) and then relay that to a servo (will be an ESC in the future). There is a lot more to do and I'm a total beginner to Arduinos and coding so the code is a mess but I'll be giving it a tidy and sort out the comments. I am getting the hang of it though and have an idea of what needs to be done. The only thing I might struggle with is scheduling the tasks so they don't interrupt each other. Hopefully I'll have time this week to tidy stuff up, add comments and give out the code I have so far. 

@Pimousse the problem running a few things at the same time is you only can process one thing at a time so if a bit of code interrupts another task it will stop things from working. Have you tried adding delays between parts of the code to slow things down? The other option is to schedule the code but reading about that means you have to do a rewrite of it all.
```

---
## \#33 Posted by: Pimousse Posted at: 2016-10-26T12:54:33.071Z Reads: 198

```
As I said, I didn't push the dev so far.
Maybe adding some delays could help. I already have one at he end of the code.
I'm not used to handle intterupts, and I read (IIRC from Vedder himself) that Arduino doesn't manage it very well.
```

---
## \#34 Posted by: PB1 Posted at: 2016-10-26T12:58:41.028Z Reads: 205

```
regarding arduino / SD Card data logger - we've been there already and @makevoid has done it already. 
See http://www.electric-skateboard.builders/t/recording-data-from-vesc-summary-of-tools/7020/9 

I would love to see the  microSD config.XML to VESC - with a slow and limited default config being loaded and then the ability to load the "hero mode".
```

---
## \#35 Posted by: Okami Posted at: 2016-10-26T13:47:43.540Z Reads: 215

```
[quote="EssEnn, post:32, topic:11900"]
My plan for the Arduino is to control the PWM signal so you can adjust top speed and apply a delayed throttle curve to the ESC.
[/quote]

So @EssEnn how much progress have you made? It seems that you have had a discussion with @DWiskow already, he is the one who has already made such a ''module''. 

Though I dont have the time and understanding to go into that now, so:

 **Can you just summarise how far have you gotten and is it easy to build such a device / module?**

**(for throttle ramping)**

---
Original thread, where @DWiskow mentioned it, is here:

http://www.electric-skateboard.builders/t/dorian-wiskow-emtb-build-trampa-holypro-17-e-toxx-belt-drive-twin-sk3-6374s-twin-max6-escs-6s-16-000mah-lipo/10859/22

----
**Would be great if he found the time and willingness to share this with others!** 

 At least from the topic alone I dont get a clear idea on how to do this myself.. unfortunately
```

---
## \#36 Posted by: Okami Posted at: 2016-10-26T13:55:36.719Z Reads: 199

```
[quote="smudgeUK, post:28, topic:11900"]
@Okami, what would be the bare minimum we should look at trying to log for the database? If we cut all the un-necessary parts off the logger (no displays etc) so it is simply recording the minimum
[/quote]


I have to check up on our initial plans for the Data base! 

We intended to collect energy use data, somer power requirements and such. 

@whitepony  went even further and advised on how it should look to make it somewhat meaningful (with charts etc)

 If I reorganise all of that stuff in somewhat readable manner I will update the old thread or make a new one!

----
Basic things would be: 

* **mah consumed**
*  **distance done**
* **average speed**
* **top speed**
* **max amp draw**
* **average amp draw**

---

From this it would be way easier to calculate **max achievable distance from battery** based on average + top speed (and average / peak amps)

Also **design suitable battery** for your needs (EG only 15mph/25kmh top speed and so on)
```

---
## \#37 Posted by: Pimousse Posted at: 2016-10-26T14:02:09.125Z Reads: 184

```
It sounds really great !!

I was wondering about how build a database for collecting datalog from VESC Monitor app.
I built a Excel sheets with macros to make the analysis fast and easy with lot's of calculated parameters (like range).
It's still in beta since I need more .txt files from longer runs than mine (1km, 3min :smile: ). 
But anyway, it could be awesome so share the file directly from the app to the database and then see charts and average data etc.

The link of Excel sheet : https://dl.dropboxusercontent.com/u/47746996/VESC%20Monitor%20Analyser.xlsm

Wait... Are we building the eskate Google ? :smile:
```

---
## \#38 Posted by: Okami Posted at: 2016-10-26T14:11:10.588Z Reads: 180

```
I have to send this to ''our programmer''. Unfortunately, at this stage I am more of a ''coordinator'' and ''inspirer'' than the one who does all the work!

---

@deathcookies is the one doing the hard work now (technical things).

 I think, to make this even further he have to contact @makevoid and some of the high experts of this forum, to progress the project further. 

As of right now we have only finished the platform, where to put all the info and text files / pictures etc.. the next step with converting files and uploading them in an easy to look at result would probably take some extra effort.. it is a question about human resources, now, I think :)
```

---
## \#39 Posted by: Okami Posted at: 2016-10-26T14:24:36.820Z Reads: 181

```
[quote="PB1, post:34, topic:11900"]
regarding arduino / SD Card data logger - we've been there already and @makevoid has done it already.
[/quote]

Would it be possible for you to summarise **what has been done so far**?

**(For reliabily recording and exporting data from vesc)**

---
I opened the thread but it is way too intense and detailed for me to start readin it now.. perhaps someone who has gone through all the thread can do the simple work of outlining:

* **How well does it work?**
* **Is it easy to set it up?**
* **What exactly is required besides Vesc, the app to make it working?**

---

Answers to all of this would be great! So far the only ''shortcut'' and easiest way to see some live data from vesc and also export it is to use the bluetooth module. So I am not so sure how much easier it is to do it on a SD card.
```

---
## \#40 Posted by: Pimousse Posted at: 2016-10-26T14:30:28.454Z Reads: 170

```
I don't have any skill in web or database coding, but I've another skill : I love to learn :slight_smile:
So if I can join the dev process, let me know.
I'm also beta-tester of VESC Monitor app and report issues to the dev.
I could be a link between both platform if needed.

There are lot's a talent guys here, but it seems that some of them work only on their own (sometimes with the hope of making money...).
If only we could all put effort together, we should be able to ride our board just with our mind. :smile:
```

---
## \#41 Posted by: Okami Posted at: 2016-10-26T14:35:37.071Z Reads: 178

```
[quote="Pimousse, post:40, topic:11900"]
If only we could all put effort together, we should be able to ride our board just with our mind. :smile:
[/quote]

ha ha :D nice future concept and something to strive for! :D 

Dunno how fast this ''brain impulse'' technology will come in everyday use, though there are some applications where it is already happening, like with the paralyzed people and such..

----

I wrote a message to @deatchookies (our dev), will see what he tells us.. though, we will probably need more than one person involved in this one.. since it was a somewhat hard toll on @deatchookies to do it alone, partly of wrong initial planning, though, **with more people in the team, this should be doable..** 

Though, I do hope that all of us (the interested parties) can come up with a plan and find a way to collaboate with each other.. will be hard if everyone is coding and doing their own project alone..

--

Some ideas and suggestion for the first initiatives on **what should be done**, would be great!

---
So far, I've got to understand how much progress have been made so far..

As of now it looks like there is:

* **Working bluetooth module**, with the option to make an app for android, too, not just iphone

* **Way to write vesc data to an SD Car**d (not 100% in tune, but that's what I understand)

* **Somewhat finished Esk8 database** for storing and displaying info with a few functions and design things still missing (should be updated&improved over time!)
```

---
## \#42 Posted by: PB1 Posted at: 2016-10-26T14:43:16.947Z Reads: 174

```
Haha, the other thread **is the summary** already ... :innocent:  suppose there is so much information in this forum now ... I only chimed in because I wanted to avoid that somebody develops code to store data on an SD card. It there already. 

In short
- there is a number of mobile phone apps available now that do logging via various bluetooth modules. For more information, please see http://www.electric-skateboard.builders/t/recording-data-from-vesc-summary-of-tools/7020/9 
- @makevoid has already developed an app that does logging on an SD Card via an arduino board. He has made the code open source. 

Here the summary again: 
Hardware: 
-	Arduino connected to VESC via UART
-	Standard SD Card shield

Code:
-	https://github.com/makevoid/VescUartControl/blob/master/examples/VescUartSample/VescUartSample.ino6

This code logs data in a JSON time series format.

Power the arduino off the VESC or use a common ground. The code runs on the Arduino device and pulls the data out of the VESC. The data is then stored on a standard SD card shield connected to the arduino. You need to set the VESC to ppm + uart mode and you only get the right data if the remote controller is on and connected.
If you want to analyze the data, the SD card needs to be removed. You can then analyze the data either using the JSON data to GIF generator or the graph tool mentioned below or some other app that understands JSON. 
If there are enough requests, makevoid might add a CSV format as output.


@makevoid also made a program that takes the JSON time series and generates a text gif to embed in videos 
Code: 
-	https://gist.github.com/makevoid/d68a4e95ba518cc84ed584afe2445f1d3

The program runs on Linux, opens the log file VESC_LOG.TXT and creates a GIF image based on the data in the log file. This image can be included in videos.

@makevoid JSON to graph app to make video overlays
Software: 
- https://github.com/makevoid/vesc-logged-data-overlay
```

---
## \#43 Posted by: PB1 Posted at: 2016-10-26T14:48:43.277Z Reads: 156

```
Suggestion (even though I'm not the OP or a moderator): 
- stick to ARDUINO help and ideas in this thread
- Love the idea of VESC logging an ESK8 DB, however there are already a lot of threads covering this topic. Please use these threads
```

---
## \#44 Posted by: EssEnn Posted at: 2016-10-26T14:53:26.478Z Reads: 165

```
@Okami That's who gave me the idea being honest, I was asking questions and not really getting much information back so I decided I'd just give it a go myself. Turns out it is not actually that difficult as Arduino's are great for outputting a PWM signal for servos. All I did was buy a starter kit from Amazon for £40 which had solderless breadboards, wires, a servo, LED's etc and get going. There are a few guides on the internet but I found a good sketch that uses interrupts to time the PWM signal from the receiver that turns out to be a lot more efficient than using the function available in Arduino ([http://www.benripley.com/diy/arduino/three-ways-to-read-a-pwm-signal-with-arduino/](http://www.benripley.com/diy/arduino/three-ways-to-read-a-pwm-signal-with-arduino/))  Writing to the servo is the easy part as there is a servo library already. The code to implement smoothing was also easy as that is available on the Arduino website. 

So right now the sketch I have will read the signal from the RX, average out the last 10 results and output the PWM pulse to the servo. The smoothing is needed as the PWM pulse from the receiver does vary slightly +/- 5 microseconds. Took me about 2 hours to actually get working but I have watched a lot of youtube video's and tons of reading (all stuff I don't fully understand) to get this far. The hardware side is piss easy as long as you remember to use a common ground. 

What needs to be done is the following - 
Setup a routine so the Arduino knows the neutral, max and min pulses from the RX (like you do with ESC's)
Write the throttle/brake ramping code (the hardest part of the project) 
Implement variable resistors to tune things like max throttle, throttle ramp speed, brake ramp speed.

Once that is working then it's easy to create different ramping curves, preset modes etc. Only thing after that would be some kind of display.

I don't mind giving people the code as it is but I have just been copy pasting chunks of code and the comments all need fixing as I have made changes. It also needs to be split into smaller functions as there is a lot going on in the loop() right now. 

@Pimousse There is probably better platform to use other than Arduino but for the cost and ease of use I quite like it. Try adding a 1 to 10 millisecond delay between the routines and see if it solves the issue. I don't think a delay that short is going to be noticeable or really affect the output.
```

---
## \#45 Posted by: smudgeUK Posted at: 2016-10-26T17:08:06.958Z Reads: 150

```
@PB1 Yes i agree, threads for specific topics should be maintained. It makes it much easier to keep track of the discussions. 
@EssEnn you know im looking forward to seeing the ideas and possibilities your project could open up. Input from the community could make this idea the next best thing for the hobby since the vesc :-)

We are still only batting ideas around here so we can just keep this one a random arduino thread with no specific direction. Any direction you want to go is a good direction!

@Okami made a good suggestion to me about a sub category for arduino, would one of the mods be able to confirm if this is something that could be looked into (or if its even possible? im sure it is) as there seem to be quite a few arduino related threads popping up and it would make it easier to keep track of them in the electronics category.
```

---
## \#46 Posted by: Okami Posted at: 2016-10-26T17:25:48.322Z Reads: 149

```
[quote="EssEnn, post:44, topic:11900"]
I was asking questions and not really getting much information back so I decided I'd just give it a go myself. Turns out it is not actually that difficult as Arduino's are great for outputting a PWM signal for servos
[/quote]

Same here. Asked in private message for more details, never got any reply :/

I think we need to develop this into somewhat ''diy kit'' or a module you can buy and install.. otherwise too many ppl dont get the chance to set their boards to ''beginner'', ''intermediate'' or ''pro'' mode..

Especially true for 10s and 12s boards, I believe, where it is quite easy to loose control and push too much of a throttle..
```

---
## \#47 Posted by: EssEnn Posted at: 2016-10-26T19:31:09.480Z Reads: 145

```
@Okami Once the code is done then anyone will be able to build one. It sounds difficult but the wiring to the UNO is well easy. If you can build a DIY esk8 then this is just as easy, just smaller. I have no idea about producing a shield for the uno for the project but looking what some people have done in this thread it can be worked out in time. First got to get the code working. I want it to work in a way that anyone can edit variables in the code so anyone can fine tune it and lastly optimise the code so it can have other functions added without affecting performance. The code is going to need to be robust as the last thing allowed is it to go haywire and hurt someone. This is the main reason all the code & designs are going to be freely available to anyone.

God I have been thinking about this WAY too much. 2 weeks ago I had never coded an Arduino and now my brain is going overdrive about it. Once things calm down at work I'll be able to actually spend some time on this as I find i'm reading a lot, thinking a lot but not doing a lot. I will be meeting a friend in a few weeks who does code C++ and Arduino's who said he would help so fingers crossed hey
```

---
## \#48 Posted by: Okami Posted at: 2016-10-26T19:55:21.862Z Reads: 143

```
Hey, that's great news! Im really happy someone has decided to make this public! (arduino code & instructions on how to fine tune the PPM/PWM signal) 

---
I first heard about this ''throttle ramping'' on an instructable about making electric scooter. The guy who wrote it had some serious background in robotics and he was also studying at MIT or a similar level school. Too bad he did not give much instructions on how to make one, though.

----

Good to hear you will get some help, I have very limited arduino knowledge, I've turned on some basic matrix displays, did ultrasonic and light sensor things, perhaps a few other little tweaks but nothing major so far.. I would appreciate if arduino code and all the instructions / functions were more easy to understand as it gets quite intense and non - understandable fast :slight_smile: 

Also takes a lot of time, patience and endurance to find what is not working! Once I spent about 3 hours to get some basic lights working :D
```

---
## \#49 Posted by: EssEnn Posted at: 2016-10-26T21:26:26.535Z Reads: 145

```
Well I had a quick look at my code and added a few comments to try and make it clear, you can grab it here - https://drive.google.com/drive/folders/0B9G-85jU01X5RUZoNGpRczRNcms?usp=sharing

I have only tested this with a servo at the other end but it does work. Pin 2 is the signal pin from the receiver and pin 3 is the transmit pin for the servo. The UNO cant supply enough juice for the receiver and is only 5V not 6V so I have 4 AA batteries in series to give me 6V. The servo seems to need to be powered from the UNO (otherwise strange things happen) and you must have a common ground or nothing works. 

I'm going to split the parts of the loop into functions and get that working hopefully tomorrow or over the weekend.

A lot of the comments are from the original writers of the code that I have copy/pasted and modified so it works. I'll compile a list of sources and add them so I can give credit where credit is due.
```

---
## \#50 Posted by: saul Posted at: 2016-10-26T21:36:52.714Z Reads: 132

```
yes thats exactly what I'm thinking. 
I just got one of the modules and I'm researching vesc/ble for an android vesc app.

Once i have the data, i might make an online tool to upload directly/compare trouble shoot...
This is all very early stage ideas tho. not sure when i'll feel like coding....
```

---
## \#51 Posted by: saul Posted at: 2016-10-26T21:41:07.576Z Reads: 140

```
[quote="Pimousse, post:40, topic:11900"]
we should be able to ride our board just with our mind. :smile:
[/quote]

is this close enough?
I think i used arduino for the wired version, so its still on topic ;)
http://www.electric-skateboard.builders/t/touchless-power-glove-control-working-interested/10718
```

---
## \#52 Posted by: ra.rend Posted at: 2016-10-26T22:10:55.822Z Reads: 139

```
I've been trying to get data from vesc via uart but still not receiving anything from the VESC. I have an arduino uno connected to a small lcd, which displays the voltage and rpm. The uno is hooked up to a lipo on the uno's 5v vcc pin and GND pin. Only the vesc's rx and TX pin are connected to the arduino.  

Could that be that problem?
```

---
## \#53 Posted by: chinzw Posted at: 2016-10-26T22:22:02.471Z Reads: 137

```
did you enable ppm+uart?
also, im not sure about this since i haven't done any vesc uart dev but i believe you have to query the vesc?

Also, its a good idea to have a common GND from the vesc to the arduino. And since the vesc can provide 5v you can just use 5v, GND, TX, RT from the vesc.
```

---
## \#54 Posted by: ra.rend Posted at: 2016-10-26T22:31:27.507Z Reads: 132

```
Yes, I have ppm+uart enabled; baud rate is also identical. 

I should add that plugging in a Bluetooth module to the VESC's uart works with the VSC Monitor app (by solarturtle?). Also, what's "query the VESC"?(Im a noob)
```

---
## \#55 Posted by: saul Posted at: 2016-10-26T22:35:36.757Z Reads: 137

```
you need a common ground forsure.

other then that I think the vesc only give data as a response. so you have to send a request code, and it will send back the data you want.

i'm not sure what the codes are yet tho... working on it.
```

---
## \#56 Posted by: ra.rend Posted at: 2016-10-26T23:07:25.587Z Reads: 136

```
Example code for.getting data from vesc and arduino library https://github.com/RollingGecko/VescUartControl?files=1
```

---
## \#57 Posted by: saul Posted at: 2016-10-26T23:10:59.117Z Reads: 141

```
vedder's blog is a good place to start too.
http://vedder.se/2015/10/communicating-with-the-vesc-using-uart/
```

---
## \#58 Posted by: chinzw Posted at: 2016-10-26T23:22:12.194Z Reads: 144

```
Are you using that?
Where did you connect the VESC's RX/TX on the arduino?
I use 2 digital pins for RX/TX since the atmega uses rx/tx pins for usb
```

---
## \#59 Posted by: domw95 Posted at: 2016-10-26T23:27:01.744Z Reads: 142

```
I am thinking of sticking an [Arduino 101](https://www.arduino.cc/en/Main/ArduinoBoard101) on my board for a bit of throttle smoothing.  Might go for a custom controller using a [Trinket](https://learn.adafruit.com/introducing-trinket/introduction) as well since they are so small

The 101 has bluetooth, a 3-Axis gyro and 3-Axis acceleromter all built in so could be perfect for data-logging, connecting to phone etc.
```

---
## \#60 Posted by: ra.rend Posted at: 2016-10-26T23:45:03.502Z Reads: 141

```
I use the serial pins on the arduino uno (pin 0/1) but  I unplug the USB. If I don't use the serial monitor on the pc and have the values output to the lcd, it should work...right? (I will test this later)

Do I really have to use Software Serial?
```

---
## \#61 Posted by: EssEnn Posted at: 2016-10-27T00:00:17.522Z Reads: 139

```
OK I just signed up for a github account and created my first repository here - https://github.com/EssEnn/esk8-Throttle-Control

I'm still trying to fully figure it all out but its a start. The name will probably change in the future and once I have something working a little more I'll probably start a thread about it. 

If anyone is able to give any advice or help, it would be greatly appreciated as I'm a total beginner at this.
```

---
## \#62 Posted by: chinzw Posted at: 2016-10-27T00:20:03.129Z Reads: 128

```
Yeah, as long as you're not using usb tx/rx pins should work fine, but its much easier to use software serial, that way you can use serial monitor for debugging and quicker code changes turnaround.
```

---
## \#63 Posted by: domw95 Posted at: 2016-10-27T00:59:20.112Z Reads: 137

```
Have you tried this code out yet?  Looks like a good basis to start.

You probably know this but interrupts can only be added to pins 2/3 on an uno so you might want to change the servo pin to 9/10 so you can add other interrupts in future :grin:

Should probably ditch the delay in your main loop for millis() compare or an interrupt.  Should prevent any problems later on
```

---
## \#64 Posted by: ra.rend Posted at: 2016-10-27T01:29:40.912Z Reads: 130

```
If I use software serial (let's say I set pin 2 as rx and pin 3 as tx and name it "mySerial"), in the "**VescUart.h**" file -- I'll have to change "#**define SERIALIO Serial**". What do I replace it with?
```

---
## \#65 Posted by: EssEnn Posted at: 2016-10-27T01:38:23.893Z Reads: 134

```
@domw95 The code as it is works but yeah i have to remove the delay and time the tasks. I actually just found this - https://learn.adafruit.com/multi-tasking-the-arduino-part-1/using-millis-for-timing after reading your post as it got me thinking. I got a good few hours on Saturday to start getting my head around this and tinkering. You are totally right about the pins and those will change as well. I was thinking about using the second channel for something but I'll focus on the core first, extras later. 

Thanks for the input
```

---
## \#66 Posted by: chinzw Posted at: 2016-10-27T06:23:26.084Z Reads: 132

```
#define SERIALIO mySerial
```

---
## \#67 Posted by: smudgeUK Posted at: 2016-10-27T07:58:49.563Z Reads: 138

```
Cheers @EssEnn ... il power up the netbook later and have a look, see if I can understand any of it. Currently making a stand for my PC PSU and accucell. Bit chilly and cloudy here today though, not sure I should charge my lipos just in case I don't make it out!
Actually found an app for android which allows you to open .Ino file and edit etc which saves me copying stuff to a .txt to mess with on my phone on the go
```

---
## \#68 Posted by: JLabs Posted at: 2016-11-22T04:06:19.517Z Reads: 139

```
Reviving this thread I need some help. I am trying to work with two HC-05 modules and cant get them to work.

I am simply just trying to get an LED to turn on from a command on the master, repeatedly send a ‘1’ to turn on the LED. I just want to get the info sent over blutooth and adapt it later.

I have the two HC-05's paired (blink together every 2 seconds) but I cant get the LED to turn on. Here is my code:

MASTER –
int state;
void setup(){
Serial.begin(9600);
}
void loop(){
if(Serial.available() > 0){ // Checks whether data is comming from the serial port
state = Serial.read();
}
Serial.write(‘1’);
delay(1000);
}

SLAVE –

 #define ledPin 9
int state = 0;

void setup(){
display.begin(SSD1306_SWITCHCAPVCC, 0x3D);
Serial.begin(9600);
}
void loop(){
if(Serial.available() > 0){ // Checks whether data is comming from the serial port
state = Serial.read();
}
if (state == ‘1’) {
digitalWrite(ledPin, HIGH); // LED ON
state = 0;
}
else if (state == ‘0’) {
digitalWrite(ledPin, LOW); // LED ON
state = 0;
}
}

Any help is greatly appreciated.
```

---
## \#69 Posted by: domw95 Posted at: 2016-11-22T08:34:03.044Z Reads: 116

```
It looks like in the Slave code loop you are resetting state to 0 every time so the led turns off pretty much immediately the next time it gets to  else if (state =='0')
```

---
## \#70 Posted by: chinzw Posted at: 2016-11-22T08:41:21.211Z Reads: 115

```
dom is right, you are not "keeping" the last state since you're redefining it to 0 for every cpu cycle.
Remove "int sate = 0;" and change "int sate;" to "int state = 0;"

Dont forget BT sends data, once, so it wont keep a 1 or 0 every time you read, just when you send that.
```

---
## \#71 Posted by: domw95 Posted at: 2016-11-22T08:51:51.040Z Reads: 124

```
Something like this should do it.  It does mean that to turn the led off you would have to send a 0 from the master, unless you put a timeout in the slave code to turn it off after not receving any more data.

    void loop(){
      if(Serial.available()){ // Checks whether data is comming from the serial port
        state = Serial.read();
        
        if (state == ‘1’) {
          digitalWrite(ledPin, HIGH); // LED ON
        }
        else if (state == ‘0’) {
          digitalWrite(ledPin, LOW); // LED ON
        }
      }
    }
```

---
## \#72 Posted by: JLabs Posted at: 2016-11-23T21:07:37.572Z Reads: 124

```
Still no luck.. Any Ideas?

**Slave**

int ledPin = 12;
int state;

void setup(){
  display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
  Serial.begin(9600);
}
void loop(){
  if(Serial.available()){ // Checks whether data is comming from the serial port
    state = Serial.read();
    
    if (state == '1') {
      digitalWrite(ledPin, HIGH); // LED ON
    }
    else if (state == '0') {
      digitalWrite(ledPin, LOW); // LED OFF
    }
  }
}

**Master**

int state;
void setup(){
  Serial.begin(9600);
}
void loop(){
  if(Serial.available() > 0){ // Checks whether data is comming from the serial port
    state = Serial.read();
}
 Serial.write('1');
 delay(1000);
 Serial.write('0');
 delay(1000);
}

PS. I am not sure how to upload code, I tried pre formatted text but it only does some of it

@domw95 @chinzw
```

---
## \#73 Posted by: domw95 Posted at: 2016-11-23T21:36:19.315Z Reads: 115

```
If you add 4 spaces in front off each line of your code it will format it like that :slight_smile:.

try putting:
    
    pinMode(ledPin, OUTPUT)
in the setup for the slave.

Also you are defining state as an **int** but in the Master you are sending a **char** as '1' or '0'.
You are also checking for a '1' or a '0' char in the slave.  Make sure the variable types are consistent.

For this it is probably easiest with char as then you are only sending a single byte.

I assume everything is wired correctly as you said you had the 2 modules paired?
```

---
## \#74 Posted by: chinzw Posted at: 2016-11-23T21:53:55.739Z Reads: 108

```
I was about to reply the exact same thing. If you don't set the pin as output, the pullup resistor will be enabled and it will limit a huge amount of current, so the LED might seem off.
```

---
## \#75 Posted by: JLabs Posted at: 2016-11-23T22:42:47.426Z Reads: 111

```
Yes the modules blink together, I made a video but it was 90mb and I have DSL so that is not a good mix. 

I will try the char and add the pin mode. Thanks a million for all of the help!
```

---
## \#76 Posted by: JLabs Posted at: 2016-11-23T22:51:23.029Z Reads: 116

```
Side note, why isint anything coming up in the slave serial monitor? I just want to know how (make sure) that the data is being communicated. Both modules blink together roughly every 2 seconds and I have went over the wiring multiple times.

New Master Code:
char state;
    void setup(){
      Serial.begin(9600);
    }
    void loop(){
      if(Serial.available() > 0){ // Checks whether data is comming from the serial port
        state = Serial.read();
    }
     Serial.write('1');
     delay(1000);
     Serial.write('0');
     delay(1000);
    }

New Slave Code:
int ledPin = 12;
char state;

void setup(){
  display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
  Serial.begin(9600);
  pinMode(ledPin, OUTPUT)
}
void loop(){
  if(Serial.available()){ // Checks whether data is comming from the serial port
    state = Serial.read();
    
    if (state == '1') {
      digitalWrite(ledPin, HIGH); // LED ON
    }
    else if (state == '0') {
      digitalWrite(ledPin, LOW); // LED OFF
    }
  }
}
```

---
## \#77 Posted by: domw95 Posted at: 2016-11-23T23:15:21.919Z Reads: 102

```
I think you are going to need to use a [Bluetooth Library](https://github.com/jdunmire/HC05) to send the Serial commands to the module

Have a look through this tutorial it should help a lot
http://www.martyncurrey.com/connecting-2-arduinos-by-bluetooth-using-a-hc-05-and-a-hc-06-pair-bind-and-link/

If you are using the hardware serial (rx and tx pins) to communicate with the bluetooth module you cannot use the usb serial at the same time.  They are the same thing so trying to send different data will mix it all up.  If you want to use the serial monitor at the same time you will have to use Software Serial for the bluetooth.

Did you actually do anything to pair the modules?
```

---
## \#78 Posted by: JLabs Posted at: 2016-11-23T23:17:51.742Z Reads: 106

```
Yes, I got the address and set one to master and slave using the AT commands. I thought that having it plugged into the computer will screw it up. I will check out the links and seperatly power both arduinos. 

Edit: just tried powering from a separate supply. No bueno. I am using 2 HC-05's so I will try it with an HC06. Thanks a lot for the pointers man.
```

---
## \#79 Posted by: domw95 Posted at: 2016-11-23T23:32:57.052Z Reads: 107

```
No problem. I'm happy to blindly suggest solutions until it works :grin:
```

---
## \#80 Posted by: rtasca Posted at: 2016-11-24T01:50:38.542Z Reads: 109

```
Currently working on an arduino sketch to read from a nunchuck thumb pot and generate a PWM signal, first wired but when my BT modules arrive, hopefully wireless. BTW the Nyko K I bought never worked... so parts will be used. 

My vesc is dead so this is going to be for a HV ESC  I got from an old helicopter that was sitting here while my DRV arrives from abroad. 

Since there is little precision from the pot,  I will implement something like cruise control, it will increase and decrease throttle smoothly and hold there when you let go. 

Just got it working fine with a test motor and esc setup.

Maybe I'm reinventing the wheel... but this is something that will work with any ESC and can use the compact form factor of a Nunchuck.

Thoughts?
```

---
## \#81 Posted by: domw95 Posted at: 2016-11-24T10:00:39.637Z Reads: 104

```
I like the cruise control idea. Probably worth using one of the rear buttons as a deadman switch that sends the ESC back to neutral when it is released otherwise things could go tits up

Going to need something similar on the receiver side that puts it in neutral if it doesnt receive a signal for a certain amount of time - already made that mistake and it wasnt good

Will everything fit inside the nunchuck ok?

I have nearly finished making my controller with a couple of nrf24l01 2.4ghz modules and Adafruit trinket pros (basically small Arduino Unos).  Shall do a post when I get time.
```

---
## \#82 Posted by: rtasca Posted at: 2016-11-24T10:07:04.541Z Reads: 91

```
Indeed the button is a very good idea, didn't think about it that way. OMG
Yeah, failsafe for sure was planned. 
The pro minis fit very well into the nunchuck ( of course w/o the headers ), just have to cut the original PCB a bit.
```

---
## \#83 Posted by: saul Posted at: 2016-11-24T10:37:31.686Z Reads: 92

```
you should also make sure you have fail safes for pins disconnecting.

I would test on a rc car or something before you rides.. thats where my nanonrf rx/tx live...
```

---
## \#84 Posted by: domw95 Posted at: 2016-11-24T12:00:27.470Z Reads: 95

```
Which pins do you mean?
```

---
## \#85 Posted by: saul Posted at: 2016-11-24T15:34:37.490Z Reads: 92

```
from the rx to the esc.

even if they are soldered, with vibration something come break and without watching for it it could trigger full brake/throttle. 
both are bad....
```

---
## \#86 Posted by: domw95 Posted at: 2016-11-24T15:58:32.507Z Reads: 85

```
Yeah I had think about this a while back and I couldn't come up anything. Once it disconnects the behaviour is completely up to the ESC so it depends what it is programmed to do. Unless anybody has any other ideas?
```

---
## \#87 Posted by: saul Posted at: 2016-11-24T16:07:31.518Z Reads: 91

```
oh thats right lol

maybe i was thinking of something on the tx side. like a disconnected pot...
those little things will get you with time...
```

---
## \#88 Posted by: domw95 Posted at: 2016-11-24T16:22:28.091Z Reads: 95

```
I've got a dead-man switch on the transmitter so hopefully that will cover it.

I have already had to chase after my board after the throttle locked on so shall be doing my best to avoid that happening again :sweat_smile:
```

---
## \#89 Posted by: saul Posted at: 2016-11-24T17:13:43.638Z Reads: 95

```
I was thinking of adding one but then I like to grip lightly when i'm going really slow...
make sure the pot is neutral when pressed, else ignore. or add ramping and you have "launch control" :sunglasses:
```

---
## \#90 Posted by: domw95 Posted at: 2016-11-24T17:37:30.751Z Reads: 98

```
I'm using an exponential moving average at the moment which smooths the throttle out nicely... until i got too cocky, jammed the throttle on full from near standstill and lent back a bit too much. :unamused:

Bit of tuning and it might be idiot proof...
```

---
## \#91 Posted by: EssEnn Posted at: 2016-11-25T12:55:24.243Z Reads: 108

```
Would you share your code for the throttle smoothing? I'm about to get back into my little Arduino project this weekend (work has been insane). 

@JLabs I did some research when starting my project and the one thing I did learn is not to use Delays if possible. Delays stop all anything from running while the delay is active so a delay of 1000 is stopping anything from happening for a whole second. In your code you have two 1000 milisecond delays. Try just removing the delays completely and see how it goes
```

---
## \#92 Posted by: ra.rend Posted at: 2016-11-25T13:59:36.353Z Reads: 112

```
You only need to use the Serial library. Look up SoftwareSerial and read this https://www.baldengineer.com/when-do-you-use-the-arduinos-to-use-serial-flush.html

The hc05s are fine. I got this working with two hc05 and 2 Arduino nano <img src="/uploads/db1493/original/3X/1/2/124a09a59097b0f258ea5e5a847a3f62a0c253cb.JPG" width="281" height="500">
```

---
## \#93 Posted by: domw95 Posted at: 2016-11-25T16:39:11.301Z Reads: 108

```
This is the main equation that does it (based on [this](https://en.wikipedia.org/wiki/Exponential_smoothing)):

    pwm_out = (int) (smooth_factor*target_pwm) + (1-smooth_factor)*prev_pwm;

There are a few issues with it at the moment.  There is a bit of a delay between getting out of neutral before the motor starts spinning.  I think I might try set a minimum output pwm and see if that helps.
There is also an integer rounding error which means it doesn't ever reach maximum.  With the current smoothing factor i think its max is about 1969ms pwm with a constant input of 2000

Other than that its seems to work quite well.

[Hopefully this should link to the files](https://drive.google.com/drive/folders/0B12vqcbFIh-cTEhwVldkZk1NQk0?usp=sharing), very much WIP but see what you think.
```

---
## \#94 Posted by: chinzw Posted at: 2016-11-25T18:43:53.793Z Reads: 100

```
That is why you should always use millis() instead of delay()
```

---
## \#95 Posted by: CaptainMerricka Posted at: 2016-11-26T06:57:52.529Z Reads: 103

```
Hey Arduino people. I have an idea I don't know how to execute. I would like to make custom led patterns for under my board. I have learned of FastLED and Adafruits NeoPixel  but I dont know which arduino/whoever board would be optimal to leave on the eboard to power some led's... I would like to be able to wire up at least one button maybe 2 to cycle the led patterns and have two led strips, 1 on each side of the board. I posted in the Eskate light thread before finding this arduino thread, and I am going to create a  thread for this arduino project so it doesn't get mixed into the others...located here http://www.electric-skateboard.builders/t/arduino-controlled-led-strips-for-underglow-fastled/13689/1
```

---
## \#96 Posted by: chinzw Posted at: 2016-11-26T07:07:34.748Z Reads: 105

```
just get a nano or a trinket, that should be enough to run your leds
```

---
## \#97 Posted by: wmj259 Posted at: 2016-12-13T02:11:00.393Z Reads: 101

```
Anyone know if its possible to replace the VESC with a arduino?
I guess not since Arduino can only handle 5V.
```

---
## \#98 Posted by: saul Posted at: 2016-12-13T02:37:23.208Z Reads: 108

```
[quote="wmj259, post:97, topic:11900, full:true"]
Anyone know if its possible to replace the VESC with a arduino?
[/quote]

possible? kinda. practical? not one bit.

This would literally "reinvent the wheel"
```

---
## \#99 Posted by: Maxid Posted at: 2016-12-13T07:32:42.662Z Reads: 106

```
http://s2.quickmeme.com/img/00/0076361a25fc3cb0d72090df1564ae81ad9aa2400c1e442589e37420ac553648.jpg
```

---
## \#100 Posted by: PB1 Posted at: 2016-12-13T16:37:31.588Z Reads: 100

```
Hmmm, yes, I suppose you could build your own ESC based on an arduino. 

You just need to 
- develop your logic and architecture of the controller (or steal it)
- develop the code (or port from other implementations)
- add a driver chip
- some mosfets
- current measurements for feedback loop
- soldier everything together or develop a custom PCB
- develop an interface to control the settings
- ...
- do some testing
- repeat all of the steps
- ...

Easy ... ;-) 

Let us know how it went
```

---
## \#101 Posted by: wmj259 Posted at: 2016-12-13T17:05:40.039Z Reads: 99

```
I love these sarcastic insults.
```

---
## \#102 Posted by: chinzw Posted at: 2016-12-13T17:39:58.914Z Reads: 97

```
A VESC and an Arduino are two completeley different things. An arduino is just an AT chip on a breakout board.
```

---
## \#103 Posted by: Okami Posted at: 2016-12-13T19:00:00.275Z Reads: 99

```
I believe you could light up a few leds or drive a very small dc motor..like for opening a cover for you.. but not really a full sized vehicle which needs to carry at least 100lbs or so :slight_smile:

Basically, I think you can look at Vedder and how much time he has spent and is still spending to create a motor controller.. You can adjust / develop control mechanism.. but to create the drive electronics is a bit different task.. I think ;)
```

---
## \#104 Posted by: PB1 Posted at: 2016-12-14T15:31:50.306Z Reads: 107

```
[quote="wmj259, post:101, topic:11900, full:true"]
I love these sarcastic insults.
[/quote]

Dont' we all? 

Suppose this is one of the drawbacks of this online world. Wouldn't be so bad if we all had a beer in our hands. 

I tried to be a bit more specific in my post. Yes it would be possible to replace a VESC with an arduino, It's just a lot of work. After all arduino is the brain of many robotics projects and is a very good interface between code and the physical electronic world. 
And yes, arduino runs on 5V. This is why we would need mosfets and potentially a driver chip to control them. 
You can even buy motor driver shields, e.g. https://www.adafruit.com/product/1438 ... up to 13,5V 
I'm not aware of standard shields that go up to our 42V. 

So yes, if anybody is up for it, it would doable and competition would be good.
```

---
## \#105 Posted by: NashTrash Posted at: 2017-01-18T03:23:17.184Z Reads: 109

```
I'm trying to create my own 2.4ghz remote system using an uno, a micro, and some nRF24L01+ modules. The only problem is that I'm a complete novice with arduino so i'm having some difficulty getting anything to work. 

I tried following some examples online but cant find anything specific to esk8 (outside of this forum of course). 

Things I want to include: dead mans switch, potentiometer based thumb wheel, data logging on the uno, and maybe lights later on.

here's what I have so far: 
<img src="/uploads/db1493/original/3X/c/c/cc9a548de90ccb0a99093924dc20a0c00df93738.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/a/b/ab29fb5983bc728d7e0233485327644b77e2888b.jpeg" width="375" height="500">

Could anyone provide a good example or tutorial on how to set these things up?
```

---
## \#106 Posted by: domw95 Posted at: 2017-01-18T10:20:31.039Z Reads: 106

```
Have managed to get the modules communicating yet?
```

---
## \#107 Posted by: mountainboardlover69 Posted at: 2017-01-18T12:15:05.220Z Reads: 106

```
hey i just made a led blink  (looks at this tread)

nope i dont know any ting
```

---
## \#108 Posted by: NashTrash Posted at: 2017-01-18T17:03:27.150Z Reads: 105

```
not yet. I'm beginning to think on of my solder joints on the chip is messed up, because I've even tried copy and pasting known working programs. Gunna have to check them over next.

Controlling the esc with the arduino is surprisingly easy on the other hand, so at least there's some progress.
```

---
## \#109 Posted by: domw95 Posted at: 2017-01-19T09:55:18.960Z Reads: 114

```
Which library are you using?  I would go for the Tmrh20 rf24 library and see if you can get the print details function to return the correct information.

I had a few issues with the arduino communicating with the module to start with.

Try follow the instructions here https://arduino-info.wikispaces.com/Nrf24L01-2.4GHz-HowTo and then run the pingpair_test  from the RF24 examples on just 1 arduino and see what it prints out
```

---
## \#110 Posted by: laikiux Posted at: 2017-02-18T19:08:27.901Z Reads: 115

```
Hi,
Maybe any of you can help me?
I can't get the values from the VESC oved uart.
There is what I have done so far:
Picked up PPM+UART in bldc tool
Set the proper bound rate to 115200
Downloaded this library https://github.com/RollingGecko/VescUartControl. (Put the folder into arduino libraries)
Done some coding.
Wired vesc5v--aruino5v vescGND---arduinoGND RX--TX TX--RX

But everything I'm not able to receive any values from the vesc.
I guess this line of code isn't working:
 if (VescUartGetValue(values))
Maybe you can help me to solve this problem?﻿
```

---
## \#111 Posted by: IsTalo Posted at: 2017-03-08T19:52:30.579Z Reads: 110

```
@smudgeUK@EssEnn @chinzw Hello, I recieved my Controller and I want to get data from it by the reciever, would it be possible?
```

---
## \#112 Posted by: Ackmaniac Posted at: 2017-03-08T20:41:23.354Z Reads: 110

```
Which kind of Arduino is it?
```

---
## \#113 Posted by: laikiux Posted at: 2017-03-09T11:23:39.495Z Reads: 110

```
It is arduino nano. And now everything works for me. But maybe you know how to calculate speed properly?
I get the rpm value. 
This is my equation:
speed=((values.rpm/2.4*0.00025136*60));
2.4 is my reduction ratio. 
0.00025136 is my wheel traveled distance per one turn (in km)
60 is minutes.
The problem is that speed is far more bigger than it would be.
```

---
## \#114 Posted by: Maxid Posted at: 2017-03-09T11:34:59.710Z Reads: 107

```
I think the rpm you get is the ERPM and needs to be divided by the motor poles count.
```

---
## \#115 Posted by: laikiux Posted at: 2017-03-09T11:37:53.598Z Reads: 104

```
My motor has 14 poles. So I need to divide it by 14?
I saw one guy divides it by 38. Why?
```

---
## \#116 Posted by: Ackmaniac Posted at: 2017-03-09T11:38:15.140Z Reads: 105

```
values.rpm / (((magnets / 2) * wheelPulley / motorPulley / (wheelsizeInMM * 3.14159265359 / 1000) * 60 / 3.6)
```

---
## \#117 Posted by: Maxid Posted at: 2017-03-09T11:38:46.566Z Reads: 107

```
I think you mean 28 - that was me :D My motor has 28 poles
```

---
## \#118 Posted by: laikiux Posted at: 2017-03-09T11:41:06.893Z Reads: 107

```
No not you :D 
@Ackmaniac why 3.6?
```

---
## \#119 Posted by: Ackmaniac Posted at: 2017-03-09T11:41:16.104Z Reads: 112

```
And if you wnat to calculate the distance then by the tachometer_abs then you need to calculate

tachometer_abs  * ((wheelsizeInMM / 1000) * 3.14159265359 / (wheelPulley / motorPulley) / magnets / 3)
```

---
## \#120 Posted by: Ackmaniac Posted at: 2017-03-09T11:41:56.714Z Reads: 110

```
Because you calculate meter per second and want km/h
```

---
## \#121 Posted by: laikiux Posted at: 2017-03-09T11:44:09.820Z Reads: 113

```
But you already did that 
revolutions per minute *60= revolutions per hour
revolutions per hour*traveled distance=km/h
Maybe I am wrong. Not sure
```

---
## \#122 Posted by: laikiux Posted at: 2017-03-09T12:11:26.883Z Reads: 113

```
The problem solved. Thank you @Ackmaniac
```

---
## \#123 Posted by: ELongb Posted at: 2017-03-28T21:15:22.870Z Reads: 116

```
Hi,
(like many) I am currently building a custom remote with OLED Display. I am using two Atmega 328p's that communicate via the NRF24L01+ modules. Sending commands with the setCurrent() (RollingGecko's library) function via UART to the VESC works, however there is a massive delay between trigger movement and motor reaction. Sometimes throttle gets stuck as well. I should probably add that I am running the Atmega 328p's at 8MHz. So my question is: Do you think the Atmega can not handle the tasks at the given clock frequency? Has anyone ever created a working (with no delay) custom remote-control based on current control? Also I don't receive any data from the VESC anymore, although I already had it working once. Baudrate, common ground between Atmega and VESC have been checked. Really losing faith in my custom solution as I literally spent dozens of hours playing with code.

Would really appreciate some help on this matter as this is for a school project.

Thanks,
Max
```

---
## \#124 Posted by: mrplaygood Posted at: 2017-03-29T07:20:40.406Z Reads: 110

```
Hi,
I've build a Remote with two arduinos and Bluetooth (not LE) and it works fine. But I have to admit that I use PWM for the acceleration and not the UART. It works really fine and has, as far as I noticed, no delay.
```

---
## \#125 Posted by: ELongb Posted at: 2017-03-29T15:26:45.610Z Reads: 112

```
@mrplaygood

Cool!
Do you run the chip at the regular 16MHz?
```

---
## \#126 Posted by: mrplaygood Posted at: 2017-03-29T18:06:18.394Z Reads: 112

```
No, I'm using a Teensy 3.2 (or LC I'm not sure) and an Adafruit Feather M0 Proto which both run at 48 MHz. These Boards are actually very fast an cheap. I would suggest that you buy one or two for prototyping. The Teensy LC cost around 12$ and the Adafruit Feather M0 Proto 20$. You don't need the Feather but it's great for battery powered projects since it has onboard LiPo charger. 
Both have full Arduino support and, when it comes to the feather, a huge community with great tutorials and libraries. And I'm not sponsored by them :D 

You could upload the code you are using. Maybe there is an unnecessary delay or something. 

Greatings
-Daniel
```

---
## \#127 Posted by: ELongb Posted at: 2017-03-31T12:54:58.875Z Reads: 113

```
@mrplaygood 
Sorry for answering so late.

This is the code I am using on the TX side:
>  #include buffer.h
>  #include crc.h
>  #include datatypes.h
>  #include local_datatypes.h
>  #include printf.h
>  #include VescUart.h
>  #include "RF24.h"
>  #include U8g2lib.h

> U8G2_SH1106_128X64_NONAME_F_4W_HW_SPI u8g2(U8G2_R0, /* cs=*/ 8, /* dc=*/ 7, /* reset=*/ 6);
> RF24 radio(9,10);
> const uint64_t pipes[2] = { 0xABCDABCD71LL, 0x544d52687CLL };
> int DisplayNumber=0;                         
> int Potpin=A0;
> struct remotePackage remPack;     
> struct bldcMeasure VescMeasuredValues;
> double persXJoy;

> enum Display 
> {
>   MainDisplay,
>   Speed,
>   Current
> };


> void DrawScreenMain(void) {
>   u8g2.clearBuffer();      
>   u8g2.setFont(u8g2_font_ncenB14_tr);
>   u8g2.setCursor(0,20);
>   u8g2.print(VescMeasuredValues.inpVoltage); 
>   u8g2.setCursor(50,20);
>   u8g2.print("V");
>   u8g2.setCursor(0,40);
>   u8g2.print(remPack.valXJoy);
>   u8g2.setCursor(50,40);
>   u8g2.print("A");
>   u8g2.setCursor(0,60);
>   u8g2.print(VescMeasuredValues.rpm);
>   u8g2.setCursor(50,60);
>   u8g2.print("rpm");
>   u8g2.sendBuffer();      
> }

> void setup() {
>   // put your setup code here, to run once:
>   Serial.begin(115200);
>   u8g2.begin();
>   radio.begin();
>   radio.setChannel(110);
>   radio.setAutoAck(1);
>   radio.enableAckPayload();
>   radio.openWritingPipe(pipes[0]);
> }

> void loop() {
>   // put your main code here, to run repeatedly:
> remPack.valXJoy=analogRead(Potpin); 
>  
>   radio.write(&remPack,sizeof(remPack));  
>   while(radio.available()){
>     radio.read(&VescMeasuredValues, sizeof(VescMeasuredValues));
>   }

>   //Display output
>   switch(DisplayNumber){
>     case MainDisplay:
>     DrawScreenMain();
>     break;
>   }
>    //Serial.println(VescMeasuredValues.inpVoltage);
> }

On the RX side the code looks like this:
>  #include buffer.h
>  #include crc.h
>  #include datatypes.h
>  #include local_datatypes.h
>  #include printf.h
>  #include VescUart.h
>  #include "RF24.h"


> RF24 radio(9,10);
> const uint64_t pipes[2] = { 0xABCDABCD71LL, 0x544d52687CLL };

> struct remotePackage remPack;                                    
> struct remotePackage lastremPack;
> struct bldcMeasure VescMeasuredValues;                                
> double persXJoy;
> int timethen;

> void setup() {
>   // put your setup code here, to run once:
>   Serial.begin(115200);
>   radio.begin();
>   radio.setChannel(110);
>   radio.setAutoAck(1);
>   radio.enableAckPayload();
>   radio.openReadingPipe(1,pipes[0]);
>   radio.startListening();
> }

> void loop() {
>   // put your main code here, to run repeatedly:


>   radio.writeAckPayload(1,&VescMeasuredValues,sizeof(VescMeasuredValues));
>   
>   while(radio.available()){
>     radio.read(&remPack,sizeof(remPack));
>     timethen=millis();
>   }
> //Serial.println(remPack.valXJoy);
>   if((remPack.valXJoy<800)&(remPack.valXJoy>300)){
>     lastremPack=remPack;
>   } 
>   else if((millis()-timethen)>300){
>     lastremPack.valXJoy=530;
>   }


>  persXJoy = map(lastremPack.valXJoy, 330, 780, 0, 250);                
>  analogWrite(3,persXJoy);
>  //Serial.println(persXJoy);
>   /*if (persXJoy > 1)                                          //Einbau eines Totbereichs
>   {
>     VescUartSetCurrent(((float)persXJoy / 100) * 10.0);              
>     else if (persXJoy < -1)
>   {
>     VescUartSetCurrentBrake(((float)persXJoy / 100) * -3.0);  
>   }*/

>   
> }

The part that takes long is probably the display output.

Greetings 
Max
```

---
## \#128 Posted by: mrplaygood Posted at: 2017-04-05T06:42:20.263Z Reads: 92

```
Hi @ELongb, sorry that I can't help right now. After Friday I'll have more time again. Hope that fits with your school project.
```

---
## \#129 Posted by: ELongb Posted at: 2017-04-08T17:06:53.527Z Reads: 99

```
@mrplaygood
Never mind!
Through tests I found out that the internal crystal of the Atmega 328p might be too inaccurate for the communication with the Vesc. 
Took me a long time to come to this conclusion.
Anyway, thank you for the help!

Regards,
Max
```

---
## \#130 Posted by: Pimousse Posted at: 2017-06-22T09:52:28.830Z Reads: 89

```
I awake this great thread to share my project with you :

https://www.youtube.com/watch?v=dxnYtA0D3gU

Remained tasks:
- Test the VESC6 UART communication (not so different from the old protocol, so should work easily).
- Adjust settings in real conditions for brightness

Once I'll consider the code finished, I'll share the Arduino Create link.
I code in a way that it should work with other LEDs configuration (e.g. bigger ring for gauge).
```

---
## \#131 Posted by: Pedrodemio Posted at: 2017-06-22T17:58:56.378Z Reads: 91

```
Nice, I've been thinking in doing something similar, in my case i want two functions, display energy consumption (average Wh/km of the ride) in a color scale, so if a can tweak my riding style if i need more range, and a battery indicator like yours

Since i'm in a long board i want something more discrete and maybe only active when a button is pressed in the remote remote

but i also have 4 LED's in my remote, just need to add few lines on the sketch, so the board indicator may be dispensable

For the brightness, a LDR and some tweaking is the way to go
```

---
## \#132 Posted by: Pimousse Posted at: 2017-06-22T19:04:21.042Z Reads: 87

```
Glad my project inspires you.
Doing your consumption gauge is not a big deal IMO.
I already thought how to integrate the ring in the nose of the board.
Just make a circle route, put the ring and cover with transparent grip ;)
```

---
## \#133 Posted by: Pedrodemio Posted at: 2017-06-22T20:39:02.646Z Reads: 83

```
Yeah, that is one way, but i wan't it to not be visible or almost non visible when off, i'm thinking a row of 3mm leds an a narrow slit in the grip tape, just enough to see
```

---
## \#134 Posted by: Pimousse Posted at: 2017-06-22T21:12:30.228Z Reads: 81

```
Could be nice also !
```

---
## \#135 Posted by: Vieo Posted at: 2017-06-22T22:10:15.631Z Reads: 79

```
How do you measure the voltage via arduino?
```

---
## \#136 Posted by: Pimousse Posted at: 2017-06-23T03:59:07.590Z Reads: 77

```
I get this info through the communication with the VESC.
```

---
## \#137 Posted by: Pedrodemio Posted at: 2017-06-23T22:15:29.876Z Reads: 77

```
Did you manage to implement the CAN forward to get data from both VESC's?
```

---
## \#138 Posted by: skelstar Posted at: 2017-12-07T23:23:30.283Z Reads: 71

```
Ok this seems like as good a place as any to ask:

I was looking at creating my version of a nunchuk using arduino (and maybe some ESP8266s) doing something similar to the RollingGecko code in talking to the VESC (very nice BTW). I wanted to simulate the nunchuk to get the "cruise control" type features, but I also wanted to get some stats/figures from the VESC as well.

From what I have worked out: the nunchul needs to talk to the VESC via i2c, and to get the stats/figures from the VESC I need to use the UART. Given that they share pins (on the VESC) this is not going to be possible.

I guess my solution now is to create my own pseudo-cruisecontrol based on the RPM that I'm reading and output an appropriate PWM signal like a normal remote from the "base" module (which connects directly to the VESC, and talks wirelessly with the controller).

Thoughts? 

Do I have it wrong? 

I've done lots of reading around here (and reading of RGeckos code) and I don't think I have seen a nunchuk/display implementation.

At the end of the day: PWM (PPM?) is not so bad... just a bit twitchy which can be addressed in arduino code (ramping./filtering).
```

---
## \#139 Posted by: Der6FingerJo Posted at: 2017-12-08T15:33:56.499Z Reads: 72

```
Hey there, i think you got most of it right, but the nunchuck doesn't necessarily have to talk via i2c. In RollingGeckos code you can see that he sends the nunchuck values over serial, so everything can work off of one serial port.
You essentially have to build a remote package and send it to the vesc. It's in ArduBoardControl if you want to see the code.
```

---
## \#140 Posted by: caprabianca Posted at: 2017-12-12T20:00:51.222Z Reads: 72

```
Hey guys, I've got some questions for you:

I am planning to make a connection between a VESC 4.10 and an Arduino UNO through the UART system I've read about in this forum. What kind of data can the Vesc send? Is it possible to read RPM if the motor is sensored? 

Second question: do I need to send PWM signals from ARDUINO to VESC if I want to control motor speed, am I right? Thanks

EDIT: I am currently reading the whole thread, in case i find some useful info and answer my questions by myself
```

---
## \#141 Posted by: skelstar Posted at: 2017-12-12T20:59:28.295Z Reads: 70

```
Have a look at RollingGecko's arduino library (https://github.com/RollingGecko/VescUartControl). 

Heaps of stats/figures can be read from the VESC. 

Also I found this library quite useful (works with ESP8266/ESP32): https://github.com/bastianraschke/ESP8266VESC

I'm currently building a VESC -> ESP32 -> NRF24 -> ESP32 (inside controller).
```

---
## \#142 Posted by: Der6FingerJo Posted at: 2017-12-12T21:09:10.558Z Reads: 68

```
Hey the ESP Library looks nice, haven't seen that until now. But it doesn't work with fw 3.xx versions, does it?
```

---
## \#143 Posted by: skelstar Posted at: 2017-12-12T21:11:28.641Z Reads: 73

```
I'm talking to one of the Turnigy VESCs (new new) which I believe are v3.10. 

I was unable to get the RollingGecko library to work but I think it's mostly because of the ESP8266 incompatibility. 

I am a little lazy and just didn't want to spend the time trying to get it to work.
```

---
## \#144 Posted by: Pimousse Posted at: 2018-05-23T09:22:51.933Z Reads: 62

```
I bring this thread back to life for a simple question : Did somebody already try to set an Arduino as a gateway between VESC and bluetooth module ?

I mean, the BT module is the master and sends commands to the VESC through the Arduino (pass through). When the VESC replies to COMM_GET_VALUES commands, the Arduino passes through but also handles the packet for some purpose (e.g. embedded LCD screen).

That way, on a single setup (= one VESC), it would be possible to display monitoring values on embedded display and still allows using an app. :slight_smile:
```

---
## \#145 Posted by: mrplaygood Posted at: 2018-05-23T10:40:00.814Z Reads: 64

```
Would you mind sketching a quick graphic how you think the communication should work? I think I did something like this but I‘m not sure yet ;)
```

---
## \#146 Posted by: Kug3lis Posted at: 2018-05-23T10:49:47.068Z Reads: 67

```
If I understood he wants UART splitter or etc so he could still send and receive data from VESC even then bluetooth is connected
```

---
## \#147 Posted by: Maxid Posted at: 2018-05-23T11:47:46.054Z Reads: 67

```
Would that also enable the use of a BT module when a Nunchuck is used? That would be awesome.
```

---
## \#148 Posted by: Pimousse Posted at: 2018-05-23T12:17:41.033Z Reads: 70

```
@mrplaygood : yes, I will. Sorry if it's not clear enough.

@Maxid : I don't think so unfortunately. Or with a heavy trick.

EDIT : Here is a drawing. Hope it helps to understand my concern.
I'd call it a VESC UART "sniffer".
![Arduino VESC UART sniffer|690x252](upload://tjWxEsAWE6oKzFRDIhSfGfs2aKx.PNG)
```

---
## \#149 Posted by: skelstar Posted at: 2018-05-23T21:08:51.827Z Reads: 63

```
I have tried this (as a replacement for using RF24, using ESP32 that has built in BT), but I'm pretty sure I was having latency issues i.e. too much of a delay.

Maybe I was doing it wrong but I rage quitted and went back to using RF24.

Also: I was trying to send objects across BT and not just using strings. Much more difficult, and the BT stack is a bit new on ESP32.
```

---
## \#150 Posted by: Pimousse Posted at: 2018-05-24T13:09:24.885Z Reads: 61

```
But if it's only for monitoring, this is not a big concern, right ?
IIRC, metr.app uses a 2Hz refresh rate.
That lets a comfortable amount of time for the Arduino I guess.
```

---
## \#151 Posted by: LittleGiant Posted at: 2019-01-26T20:21:10.554Z Reads: 37

```
Hello, I`m doing an  automated electric skateboard project and this seems like a good place to ask.
The idea is to add some sensors via arduino. Is it possible to connect arduino to VESC UART port and send signals from arduino to VESC? As far as I researched, there are projects to read pwm from vesc, but I want to send signals, for example to slow skateboard down. Sorry for my english :slight_smile:
```

---
## \#152 Posted by: skelstar Posted at: 2019-01-27T23:42:45.507Z Reads: 32

```
Yes there definitely is.

Go [here](https://github.com/RollingGecko/VescUartControl) and [here](https://github.com/bastianraschke/ESP8266VESC). There are many projects on here that do this as well.
```

---
## \#153 Posted by: Slak Posted at: 2019-01-29T13:00:23.770Z Reads: 27

```
There is not a lot of project doing what you want to do (send signals to VESC) but I know someone did a cruise control mode on his remote and I guess it send signals to VESC. The problem I see doing this is "reliability" (what if something goes wrong and the board accelerates in the middle of a crowd ?)
```

---
