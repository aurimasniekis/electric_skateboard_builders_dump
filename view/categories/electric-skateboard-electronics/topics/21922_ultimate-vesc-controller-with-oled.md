# Ultimate VESC Controller with OLED

### Replies: 150 Views: 10443

## \#1 Posted by: lox897 Posted at: 2017-04-27T21:36:10.150Z Reads: 813

```
Hey ESK8ers,

I created this thread to document progress on the VESC remote I am making. It will be fully open sourced once I have finished and tested it. Waiting on an NRF right now 😞

Anyway here are the specs:
NRF24L01 for communication
0.96" OLED Display showing speed, battery data etc
Custom 3D printed case
Thumb wheel mechanism I designed to attach to a cheap joystick

Here are some pictures of the progress so far:
<img src="/uploads/db1493/original/3X/f/1/f1bc5db8b5b21e09b6d2cf291e61f5d307a15027.PNG" width="516" height="499"><img src="/uploads/db1493/original/3X/9/9/9980560bf16fc0364482a1f3e693e63e6928fb84.PNG" width="517" height="500">

The code is RollingGecko's, he deserves all of the credit for the software side of things. I have designed the trigger mechanism and the case for the whole thing. I will be releasing the case and trigger designs in the future under a CC license that allows you to make them and even sell them as long as you credit me (would love some input if this CC license exists).

Peace guys, and I hope to have some updates as soon as Yanwen deliver the NRF. Feel free to make some suggestions or ask any questions down below.
```

---
## \#2 Posted by: Stefan Posted at: 2017-04-27T21:58:13.960Z Reads: 691

```
Are you going to use an arduino nano for communiction with the nrf?
```

---
## \#3 Posted by: lox897 Posted at: 2017-04-27T22:13:27.602Z Reads: 681

```
Yes, the Arduino nano is connected to the OLED and NRF
```

---
## \#4 Posted by: Stefan Posted at: 2017-04-27T22:15:58.431Z Reads: 663

```
Is there a was to do it with arduino pro minis? I tried it but as soon as i tell the programmer i want to upload the code to a arduino mini it will not compile without errors..
```

---
## \#5 Posted by: Eboostin Posted at: 2017-04-27T22:22:39.507Z Reads: 642

```
Nice!

Looks like a slightly larger benchwheel remote
```

---
## \#6 Posted by: Dornacht Posted at: 2017-04-27T22:27:23.644Z Reads: 612

```
@lox897 will it be possible to customize the remote more with switches for turning on lights, turn signals, brakes, I  want an ultimate esk8 remote
```

---
## \#7 Posted by: lox897 Posted at: 2017-04-27T22:38:35.503Z Reads: 591

```
Yeah I designed it based on the benchwheel remote
```

---
## \#8 Posted by: lox897 Posted at: 2017-04-27T22:42:43.348Z Reads: 582

```
I believe RollingGecko used minis at the start. Pretty sure you had to change something in the code for the minis.
```

---
## \#9 Posted by: lox897 Posted at: 2017-04-27T22:44:09.968Z Reads: 578

```
RollingGecko hasn't implemented that feature yet, but I'll look over the code when I find time and see if I can figure out how to put that in. Anyone on the forum know a bit about Arduino and NRF communication?
```

---
## \#10 Posted by: rpn314 Posted at: 2017-04-28T00:04:10.788Z Reads: 578

```
[quote="Dornacht, post:6, topic:21922, full:true"]
@lox897 will it be possible to customize the remote more with switches for turning on lights, turn signals, brakes, I  want an ultimate esk8 remote
[/quote]

Something like that is definitely possible. Vedder has some vode in place to handle turn signals and brake lights. For anything more than that the standard VESC firmware would have to be modified or there would have to be an control board (Arduino or something) that would go in between the VESC and NRF module that would handle the extras and then forward everything else onto the VESC.

[quote="lox897, post:9, topic:21922"]
Anyone on the forum know a bit about Arduino and NRF communication?
[/quote]

I've done some. Are you looking for something specific?
```

---
## \#11 Posted by: makevoid Posted at: 2017-04-28T00:28:16.956Z Reads: 524

```
nice! 



(10c)
```

---
## \#12 Posted by: ACIN Posted at: 2017-04-28T00:36:32.148Z Reads: 505

```
Will the electronics support custom modification like extra switches on remote for LED lighting?
```

---
## \#13 Posted by: rpn314 Posted at: 2017-04-28T01:22:59.043Z Reads: 524

```
[quote="ACIN, post:12, topic:21922, full:true"]
Will the electronics support custom modification like extra switches on remote for LED lighting?
[/quote]
Answer:
[quote="lox897, post:9, topic:21922, full:true"]
RollingGecko hasn't implemented that feature yet, but I'll look over the code when I find time and see if I can figure out how to put that in.
[/quote]

The other thing I would LOVE is a bluetooth connection in the remote (not for the main connection to the VESC but to connect to other devices like a phone). This would allow those who only have a single motor setup to get full telemetry recording and use the cool apps and video overlay type things.
```

---
## \#14 Posted by: ACIN Posted at: 2017-04-28T01:55:06.298Z Reads: 471

```
Ha sorry its 4am here in Germany so I was too tired to see :sweat_smile:
```

---
## \#15 Posted by: Dornacht Posted at: 2017-04-28T02:36:51.468Z Reads: 488

```
I think the functions that are most needed in the "Ultimate remote:
would be:
-switch legs for
    -Turn signals
    -brake light
    -front beam lights
    -underglow board light
-servo leads 
external disk brake and other fun
and a beginner switch so friends can try your board
```

---
## \#16 Posted by: lox897 Posted at: 2017-04-28T04:02:03.263Z Reads: 471

```
I don't think the UART port will work with two communication modules. Maybe one on the master and one on the slave VESC?
```

---
## \#17 Posted by: chsknight Posted at: 2017-04-28T04:30:02.723Z Reads: 459

```
How reliable can we expect the NRF24L01 to be?
```

---
## \#18 Posted by: rpn314 Posted at: 2017-04-28T04:30:20.641Z Reads: 465

```
I'm sure it'll work. You just have it forward any requests to the vesc and then back to the Bluetooth device. That was the premise of the nunchuck controller that @jacobbloy was working on about a year ago (ended poorly for non-technical reasons....its not worth looking up)
```

---
## \#19 Posted by: rpn314 Posted at: 2017-04-28T04:33:17.916Z Reads: 460

```
With the amplified antenna module I have, its been quite reliable, but full disclosure, my NRF connection died on me about a week ago...and hasn't come back (ie it wasn't just a short dropout).... I'm still working on it. I think my vesc has an issue, but I'm not sure yet.
```

---
## \#20 Posted by: jacobbloy Posted at: 2017-04-28T05:02:21.285Z Reads: 506

```
If you are pairing an app and a Bluetooth remote the remote and phone are the ones searching and connecting to the module on the vesc so you can use both but not at the same time. 

Using both vesc work. You can't use nrf and uart at the same time sadly. This is the reason why I chose to use Bluetooth for the remote.

Benjamin hasn't worked on it for a long time but his remote works great if using genuine chips on the nrf boards. I would like to just use 1 of the micro ppm or sbus receivers that I use every day for FPV quads and they support telemetry. The benifit is you have binding protocols that work great like AFHDS Used by flysky and the Frsky protocols. You can buy a 4in1 diy module from banggood that has support to connect to over 22 different RC receivers and has telemetry support. That youcan use on any hobby receiver. It's also 100% opensource so based on arduino so that you can implement it your self.

https://github.com/pascallanger/DIY-Multiprotocol-TX-Module

Then add simple analog to ppm code to the arduino code, 

https://github.com/fishpepper/analog2ppm

you can then add upto 16 analog switches and buttons or pots.

These analog signals get inputed into the multiprotocole modle code ppm input it then sends it to the RC receiver.

If I get time I'll try and join the 2 code structures that that the 1 arduino board just has a few analog inputs and then there is no need for the ppm input.

Also you don't need to have all 4 RF modules you can simply choice one.
```

---
## \#21 Posted by: rpn314 Posted at: 2017-04-28T06:38:34.628Z Reads: 444

```
Good to see you around here again! That's some fantastic information!

My thought (and what I thought you had been working on a year or so ago) was to have an NRF (or the micro ppm or sbus based connection between the controller and the vesc for reliability and then a Bluetooth connection between the controller and a mobile device (Bluetooth because of the widespread availability/compatibility of Bluetooth) for added viewing, recording, and maybe even configuring. Are you saying that's not possible?

I'd like to look into the micro ppm and sbus modules you referred to. Is that something like this?

https://m.banggood.com/2_4G-8CH-Micro-Frsky-D8-Compatible-Receiver-With-PPM-SBUS-Output-p-1104843.html
```

---
## \#22 Posted by: Print3r Posted at: 2017-04-28T06:48:19.163Z Reads: 419

```
Exactly what I had been looking for - both the NRF24L01+ for communication and a screen! How are you measuring current draw and voltage, is this ouputted through uart from vesc?
```

---
## \#23 Posted by: lox897 Posted at: 2017-04-28T07:03:29.927Z Reads: 404

```
Yes it is outputted through UART from vesc. Same as any of the bluetooth vesc apps
```

---
## \#24 Posted by: paragon Posted at: 2017-04-28T07:09:21.375Z Reads: 413

```
I have an early version of that module in my Devo tx :sunglasses:
```

---
## \#25 Posted by: lox897 Posted at: 2017-04-28T20:33:44.676Z Reads: 400

```
The best part about this remote is that I made it for under $20 AUD, you can get most of the parts off AliExpress or ebay for really cheap.
```

---
## \#26 Posted by: Okami Posted at: 2017-04-28T22:48:27.059Z Reads: 396

```
@lox897  So can you ''port it'' in an easy to do list?

If I buy the right stuff and arrange it together, will I be able to use your code for the remote?

I know you said contribution goes to Rolling Gecko Libraries or such.. but still
```

---
## \#27 Posted by: lox897 Posted at: 2017-04-29T00:59:39.865Z Reads: 385

```
Yes I will make a build list soon. I take no responsibility for the use of my designs, or any of the software and parts. If anyone injures themselves, please know you built this at your own risk. I may even make a video today on my new PC 😁
```

---
## \#28 Posted by: Sander Posted at: 2017-04-29T01:44:29.601Z Reads: 386

```
Funny to see controllers with oleds now.
I have been working with mine for over 1 month ;)
Mine has a menu with options like change the light color, speed, acceleration, max amp etc. 
And like yours, showing battery voltage and avg motor ampere :slight_smile:
Soon I will have a gps in my board that will log the location and give me the current time zone, so I can see on my remote what the time is instead of taking the phone out of the pocket.
```

---
## \#32 Posted by: kptheinventor Posted at: 2017-04-29T03:39:46.895Z Reads: 399

```
This is sick!!! Are you planning on selling them yourself when you finish?
```

---
## \#33 Posted by: lox897 Posted at: 2017-04-29T03:40:48.349Z Reads: 410

```
I'm still in school right now and don't have the time to build these. But I hope me open sourcing it and allowing people to sell it will help out
```

---
## \#34 Posted by: lox897 Posted at: 2017-04-29T03:54:52.752Z Reads: 416

```
Here's the video @Okami
Please subscribe to my channel on ESK8 and CAD tutorials.
https://youtu.be/ZxhG3mYfBdw
```

---
## \#37 Posted by: rpn314 Posted at: 2017-04-29T04:04:58.190Z Reads: 403

```
I was halfway through watching that! ;P
```

---
## \#38 Posted by: lox897 Posted at: 2017-04-29T04:12:28.142Z Reads: 392

```
Uploaded check above
```

---
## \#39 Posted by: Sander Posted at: 2017-04-29T04:12:56.346Z Reads: 394

```
But one question why are you using a SPI OLED display? Why not I2C OLED display? With the I2C you only gotta worry about 4 pins, GND, VCC, SCL, SDA. And with SPI its like 6 pins...
```

---
## \#40 Posted by: lox897 Posted at: 2017-04-29T04:13:27.508Z Reads: 382

```
That's what RollingGecko used and said was supported
```

---
## \#41 Posted by: Print3r Posted at: 2017-04-29T09:10:16.075Z Reads: 383

```
I agree that an I2C display would be better pinwise - it also means the screen pcbs are smaller as there are less pins. This would be very useful for me as I am going to make next year a controller with a display angled like an HTC vive controller being held with the trigger upwards. I like the idea of the boosted wheel replacing the top of the joystick, but am wondering if there is not too little travel in a joystick. Finally, is variable braking power (like variable throttle) supported in RollingGecko's code?
```

---
## \#42 Posted by: lox897 Posted at: 2017-04-29T09:23:45.272Z Reads: 373

```
Not sure why RollingGecko didn't go I2C... I'll test the travel of the joystick once my 3d printer is finally up and running. What do you mean by variable throttle?
```

---
## \#43 Posted by: Print3r Posted at: 2017-04-29T14:08:52.231Z Reads: 385

```
When you have an esc (e.g. on an rc plane) you can control the speed of the motor using that esc. I would like to be able to do the same with reverse (if a certain button is pressed) and have pulling back on the throttle past the neutral point to be increasing braking force. I have not yet bought a Vesc so do not know how to do that (for the moment)! Has anyone tried contacting RollingGecko on this forum for input?
```

---
## \#44 Posted by: nmagz3 Posted at: 2017-04-29T14:52:46.209Z Reads: 377

```
The progress you've made so far is so awesome!  Love the innovation.  Can't wait to see the final product.
```

---
## \#45 Posted by: lox897 Posted at: 2017-04-29T22:16:22.075Z Reads: 375

```
The VESC can do that. I believe you mean when you brake and go back to a standstill then you can reverse?
```

---
## \#46 Posted by: ACIN Posted at: 2017-04-29T23:36:09.025Z Reads: 349

```
The Dream :stuck_out_tongue: :heart_eyes:
```

---
## \#47 Posted by: lox897 Posted at: 2017-04-30T01:48:46.757Z Reads: 377

```
Don't like wires
<img src="/uploads/db1493/original/3X/5/1/51ac53e3de705c837d05dfa448d55599194f5eae.PNG" width="503" height="500">
```

---
## \#48 Posted by: lox897 Posted at: 2017-04-30T06:07:55.819Z Reads: 371

```
A little update on the LED button situation:
I have researched deeper into adding a button to the remote which allows LEDs to be triggered on the board.
http://www.elec-cafe.com/nrf24l01-basic-control-led-arduino/
http://www.instructables.com/id/Wireless-Remote-Using-24-Ghz-NRF24L01-Simple-Tutor/
We could probably include one of these in the code somewhere, and have the LED and analog joystick data sent over the same NRF.
It may mean modifying the code a little bit to work alongside the remote.
```

---
## \#49 Posted by: Print3r Posted at: 2017-04-30T06:51:05.826Z Reads: 367

```
I think having this ability would be cool but not essential - it is not like you are going to be in such a rush that as soon as it gets dark you don't have the time to stop, flick a switch on the board to activate the LED circuits (brakes, headlights and general under-board glow). I am wondering if the extra data (going in both directions) will make there be more errors? Don't know. I am sure everyone would find an extra channel useful at some point!

Back to what I was saying earlier, I will detail my idea for the code more clearly:

* button1 = reverse button (located somewhere where you won't hit it accidentally
* button2 = arm button (when pressed you can move around, when not pressed the board doesn't move)
* joystick = accelerate if pushed in direction of where you want to move and brake to standstill if pushed in opposite direction to where you want to move (if you are facing the board and want it to reverse, you press reverse button, pull the stick towards you and then push the stick forward when the board is right by you)

Features I may add next year when I have more time:

* GPS + app --> using google API on phone, get a list of instructions for where to go, extract the data needed (turn left/right/ which exit/ straight on + location to move onto next instruction), send that data over bluetooth and store it on EEPROM/ sd card on controller, have a bitmap for each of the turn signals and a cheap GPS (running at really low speeds eg 1Hz - conserves energy and means you don't have to get a very expensive, powerful gps chip) that measures the location so that the controller knows when to move onto the next direction. This may require more arduinos - I know that there are not infinite UART inputs, so may store the directions on one arduino that runs the GPS and bluetooth, have it send a high on a digital output to another arduino - to indicate that the next instruction should be shown. Will need feedback on how this could be done best!

* LEDs on the controller so that it also functions as a torch if skateboarding at night - this can be hardwired so won't need to use up more I/O pins.
```

---
## \#50 Posted by: lox897 Posted at: 2017-04-30T07:17:44.882Z Reads: 331

```
RollingGecko already has code implemented for a reverse button. An arm button would be very simple. I'm liking the form of a nunchuck more and more. Would be so much easier with the reverse button, arm switch, and joystick. Maybe the arm button could go where the boosted arm button is. Could even be a momentary power button (the one that is only on if held). I don't get the point of the LEDs either, but I guess generally another button to trigger something would be nice. Maybe a horn, turning signals etc
```

---
## \#51 Posted by: Print3r Posted at: 2017-04-30T07:33:41.547Z Reads: 350

```
I agree with the location of the button (like the boosted board 'engage' button) and think that it has to be momentary - the board must stop quickly if the controller flies out of your hand if you fall. There should also definitely be a check that if the button is not held for less than 0.5s, the Tx and Rx both understand that is an error in communication. If the button is not held for more than 0.5s the board should slow down. I really like the deign of the nunchuck but would like to have a display on the front of the controller, that can be glanced at while riding and would like the antenna to be on the other side of my hand (especially considering that people got some no-signal issues with the first nunchucks a year ago). I have also found that the cheapest boards with antennas and amplifiers (http://www.ebay.co.uk/itm/NRF24L01-PA-LNA-SMA-Antenna-Wireless-Transceiver-communication-module-2-4G-1100m-/201701854993) are not that much more expensive than the one with the onboard antenna. Using a truck-horn installed under an esk8 in a traffic jam would be funny!
```

---
## \#52 Posted by: lox897 Posted at: 2017-04-30T12:39:51.304Z Reads: 323

```
Please subscribe to my YouTube channel. There will be another update later this week on the case design and trigger mechanism. I'd also like to know how many people are interested in buying one of these (I won't be selling them yet (maybe never) just would like to have an idea of interest). This data could also help other people who might want to sell them if they decide to make one.

Once I have the prototype working, I will be testing it with local ESK8ers to see what they think
```

---
## \#53 Posted by: kptheinventor Posted at: 2017-04-30T12:48:49.339Z Reads: 311

```
I could be keen to buy one/ help test prototype
```

---
## \#55 Posted by: lox897 Posted at: 2017-04-30T13:09:52.358Z Reads: 332

```
Forgot to make poll public so please vote again
[poll public=true]
- Interested in this remote
- Not interested in this remote
[/poll]
```

---
## \#56 Posted by: Print3r Posted at: 2017-04-30T14:54:01.788Z Reads: 359

```
I will be making a transmitter as well probably based on the software you are using, but different design. If they work, they are certainly very cheap to produce (depending on the manufacturing process for the shell) so selling a reliable one will be no problem ... I think. If the software is made really good it could also be easily put in a new shell and have the NRF24L01+ modules taken out (replaced with wires) and sold for the Ebike community as well. I think first thing to focus on is software and design though! Kickstarter has shown that anything with marketing can be sold and this forum has shown that any good, open-source Eboard product will be bought to support the community.
```

---
## \#57 Posted by: lox897 Posted at: 2017-05-01T12:00:50.432Z Reads: 371

```
Updates on enclosure design. Changed it to a circle for the finger hole, looks much cleaner IMO. Added thumb wheel. <img src="/uploads/db1493/original/3X/e/e/eef8a7dfcc63f73f5a40d8bb52a659e577c41d20.JPG" width="281" height="500"><img src="/uploads/db1493/original/3X/c/8/c8b7db9078aa770c0becab9e24f28a23069b1f42.JPG" width="281" height="500">
I've also ordered parts for five remotes which I am undecided what to do with yet. Once I finish them I MAY get some beta testers. Ordered the joystick and some new NRFs with external antenna
```

---
## \#58 Posted by: Print3r Posted at: 2017-05-01T13:11:09.486Z Reads: 344

```
Do the antennas have a power amplifier circuit?
```

---
## \#59 Posted by: lox897 Posted at: 2017-05-01T20:44:31.120Z Reads: 334

```
Not sure. Here is the link to the one I bought: http://s.aliexpress.com/j6FBJZRz
```

---
## \#60 Posted by: Sander Posted at: 2017-05-01T22:12:13.542Z Reads: 341

```
The remote looks beautiful! You should add a fillet on the circle your finger goes through on the remote if not you will notice some pain in your finger ;)
```

---
## \#61 Posted by: lox897 Posted at: 2017-05-01T22:24:18.421Z Reads: 334

```
Great idea! I will add a curve on there. Will be doing some videos later this week on the remote. Looking forward to all the parts coming so I can make the prototype
```

---
## \#62 Posted by: kptheinventor Posted at: 2017-05-01T22:40:04.479Z Reads: 333

```
Well done, keep up the good work.  Looks really good!
```

---
## \#63 Posted by: Print3r Posted at: 2017-05-02T06:02:18.069Z Reads: 327

```
Looks like it does - you shouldn't have signal cut-outs then! Where is the antenna going to come out? or is it all in the case?
```

---
## \#64 Posted by: lox897 Posted at: 2017-05-02T06:22:15.304Z Reads: 327

```
I'll figure that out once I get it. Need to have all the components so I can start test fitting. Maybe along the side of the case or under the finger hole bit
```

---
## \#65 Posted by: Print3r Posted at: 2017-05-02T09:27:43.840Z Reads: 330

```
I have made a replica of a 2.4ghz wifi antenna on fusion 360: http://a360.co/2pxvXCb - anyone can use it if they need it.
```

---
## \#66 Posted by: lox897 Posted at: 2017-05-02T10:56:27.016Z Reads: 331

```
Thanks! I might work on test fitting some components in there. I feel like the joystick might be a bit bigger than I thought so I might have to make the case a bit larger
```

---
## \#67 Posted by: lox897 Posted at: 2017-05-02T13:15:55.955Z Reads: 312

```
I'd also like to add a button to change to beginner mode. This might tell the Arduino to divide the analog joystick reading by two to limit to half throttle (not sure that's possible), or changing vesc settings. Although RollingGecko's code is all reading data and no writing, so the first option will be better if I can figure it out. Also just joined a thing at my school with lots of access to arduinos, joysticks, NRFs etc, so I can improve my coding skills and try and figure out this beginner mode for you guys.
```

---
## \#69 Posted by: lox897 Posted at: 2017-05-02T21:30:45.451Z Reads: 293

```
Lol don't get yourself banned James. This forum's for electronic stuff, not gasoline cars.
```

---
## \#70 Posted by: wmj259 Posted at: 2017-05-02T21:40:07.529Z Reads: 296

```
How much would it be for beta testing?
```

---
## \#71 Posted by: lox897 Posted at: 2017-05-02T21:55:19.597Z Reads: 297

```
I will get the final prices for all the products combined soon. I can't promise anything until I have 5 working prototypes. But it will probably be $30-$40
```

---
## \#72 Posted by: lox897 Posted at: 2017-05-03T20:16:27.040Z Reads: 295

```
NRFs arrived! But I don't have any male to female jumpers so will have to wait a week for those. Grrrrrrr
```

---
## \#73 Posted by: sprocket12 Posted at: 2017-05-03T22:40:34.371Z Reads: 298

```
Sign me up!
```

---
## \#74 Posted by: lox897 Posted at: 2017-05-06T07:23:43.463Z Reads: 305

```
Where do you guys want buttons to be? On the front near the oled? If you put your index finger through the hole, then your thumb will be on the thumb wheel, the rest of your fingers could control buttons on the bottom left. The two buttons will switch from forward and reverse, and cruise control. You will also be able to move the thumb wheel left and right to change the display on screen (something I found out from @Print3r ), I always saw the multiple screens and didn't figure out until today that they were switched with the joystick. @Print3r could you please link the spot you saw that?
```

---
## \#75 Posted by: Print3r Posted at: 2017-05-06T08:30:27.604Z Reads: 319

```
Here is the link:
https://github.com/RollingGecko/ArduBoardControler/issues/1

Where is the oled going (can you send some picture of where you are thinking of putting it)? Though I have a tendency to make controllers larger than some would like, I do not think that screen controls should be placed out of reach of where your hand will normally be whilst riding - you should focus on your speed and surroundings not changing the display whilst riding. Buttons like arm/ disarm should be placed under the fingers I think so that when you grip the controller, they are activated. Else, the reverse button and arm button should be placed like on the nunchuck controller.
```

---
## \#76 Posted by: lox897 Posted at: 2017-05-06T09:07:55.502Z Reads: 335

```
Planning to have it a bit like this. My 3D printer is so close to being fixed, bloody thermistor or heating element isn't working yet. Aargh. <img src="/uploads/db1493/original/3X/d/7/d793910a6a608561045460eaead4f4ab2bfeb1de.jpg" width="375" height="500">
```

---
## \#77 Posted by: Mike_Lemon Posted at: 2017-05-06T17:52:36.962Z Reads: 313

```
Did you manage to read the data off the VESC from the board that connects to it through software serial?
if so please share the code thanks in advance.
```

---
## \#78 Posted by: petter Posted at: 2017-05-06T21:46:02.531Z Reads: 303

```
Count me in for testing! Also this is my sort of project, have the skillz to move it forward if there is any snags. Also have a working prusa mendel for prints and CAD skill so i might do my own enclosure, i have the nano X right now but im not super fond of the shape. Its alright but i had the nunchuck before, just so much better and ergonomical. I would go for that general shape, maybe bigger.
```

---
## \#79 Posted by: lox897 Posted at: 2017-05-06T22:25:20.203Z Reads: 305

```
It's reading data through an Arduino nano and a nrf module on the VESC and transmitter side
```

---
## \#80 Posted by: saul Posted at: 2017-05-07T05:27:04.565Z Reads: 326

```
this is not completely related since I won't be using rg's code, yet. but it should be fully compatible with an i2c oled. 

these are 2 versions of the same pcb, about to order a few to test. nano's are small but wires are not.
these are using the atmega328p pu. all through hole parts so easy to solder. and very diy looking. and very compact. the first is pro mini size. the second is only 13mm x 60mm. but the nrf hangs off + 25mm

<img src="/uploads/db1493/original/3X/c/8/c8279596eb157701def43f2b73f0800f5e923768.png" width="246" height="500">
<img src="/uploads/db1493/original/3X/9/e/9e3929f7c32da12357959bcb61eaacb5b888771e.png" width="107" height="500">
```

---
## \#81 Posted by: lox897 Posted at: 2017-05-07T07:46:49.820Z Reads: 283

```
Nice, I'm already working on a pcb though that connects nano, oled and nrf. That will be for future versions though.
```

---
## \#82 Posted by: Mike_Lemon Posted at: 2017-05-07T11:20:20.884Z Reads: 290

```
Yeah but is it using the hardware serial pins or some other pins?
```

---
## \#83 Posted by: lox897 Posted at: 2017-05-07T20:08:21.341Z Reads: 293

```
It's using the UART pins on the VESC
```

---
## \#84 Posted by: lox897 Posted at: 2017-05-12T21:45:15.459Z Reads: 304

```
UPDATE: extended range (1100m) NRF modules came in, as well as the joysticks. I know you're not going to be more than 2-3m away from your board but this should provide a very strong signal. I'll order the jumpers locally soon to get the breadboard prototype fully working! The joysticks were bigger than I thought so I'm still considering a different case design (maybe nunchuck or steeze style, or just make current one bigger.
```

---
## \#85 Posted by: kptheinventor Posted at: 2017-05-12T22:35:59.206Z Reads: 307

```
That's real good you want to know your signal is reliable :slight_smile:
```

---
## \#86 Posted by: lox897 Posted at: 2017-05-13T07:22:49.808Z Reads: 319

```
https://instagram.com/p/BUBh5XQgtSD/
Joystick working! Ordered jumpers that will be here in a week or two then I'll be using a breadboard remote for testing haha
```

---
## \#87 Posted by: zk8_builder Posted at: 2017-05-13T07:25:27.282Z Reads: 300

```
So good, keep it up
```

---
## \#88 Posted by: lox897 Posted at: 2017-05-13T07:55:21.711Z Reads: 285

```
Thanks for the encouragement dude! Appreciate it
```

---
## \#89 Posted by: zk8_builder Posted at: 2017-05-13T08:17:28.709Z Reads: 289

```
No problem, Aussies got to stick together
```

---
## \#90 Posted by: ACIN Posted at: 2017-05-13T10:32:13.915Z Reads: 296

```
That looks great, really stoked for the NFC stuff!
I would maybe move the buttons a bit apart, but we have to test it in our hands to see.
Nunchuck I think would be even better ergonomically (and suited not just for the righthanded) but you'd have fit the screen in somehow, which I think would have to go above the joystick.
Might find the time to do a little sketch of what I mean and look if that would work out, if you are still open for a different form.
```

---
## \#91 Posted by: lox897 Posted at: 2017-05-13T10:52:56.680Z Reads: 280

```
Yeah I'm really into the nunchuck idea, mainly due to it's form factor and the buttons already on the front for cruise control. Then maybe just put the screen on the side.
```

---
## \#92 Posted by: lox897 Posted at: 2017-05-13T11:19:40.292Z Reads: 276

```
Ordered a nunchuck to dremel and test
```

---
## \#93 Posted by: lox897 Posted at: 2017-05-13T14:12:20.957Z Reads: 282

```
Added channels to allow joystick to go left and right (only when you try) so you can change screen modes. Added hole so joystick PCB fits into case nicely
```

---
## \#94 Posted by: lox897 Posted at: 2017-05-13T14:14:04.504Z Reads: 281

```
Also contacted Maytech to see if I can buy the steez remote cases by themselves.
```

---
## \#95 Posted by: zk8_builder Posted at: 2017-05-13T21:58:14.788Z Reads: 265

```
Did you not like the design you made?
```

---
## \#96 Posted by: lox897 Posted at: 2017-05-13T22:50:28.311Z Reads: 274

```
I've improved the design I made but looking at different options as well. Nunchuck, steez, and custom design
```

---
## \#97 Posted by: RollingGecko Posted at: 2017-05-28T22:19:38.709Z Reads: 297

```
Hi Guys,

I just have seen this thread and I'm happy to see, that my project is continued her! 
I'm now running my remote a year without any issues. I had some problems with the reliability of the nRF24 RF link. I solved it by adding an external antenna to it.
There was the question why I was  not using I"C for the oled. I tried a lot of oleds and hat a lot of trouble with it. Finally I found one, that worked. It was not with I2C. But that can simply be added in the code.
Once it was also planned to add a configuration of the vesc over the remote. But that requires a lot a changes in the used protocol because it requires a bidirectional communication. I use the acknowledgement package that sends the nrf24 back for every revived message. With each control package send to the board, the receiver site sends the telemetry data back. If you are going now to establish a bidirectional communication, you have to establish a protocol as additional layer on the protocol used by the nRF24. All the communication to the VESC must be managed by the remote site. That is a safety issue is still didn't solve. Though I started in my VescUartControl library already on a DEV branch some changes in this direction. Maybe somebody wants to take a look at it and find a solution. 
[https://github.com/RollingGecko/VescUartControl](https://github.com/RollingGecko/VescUartControl)
As far as I have seen, Vedder implemented on the VESC a nRF24 communication. But I didn't checked that out yet.

My main issue is time. I'm already deep in other projects and can not find the time to continue the project. So any contributor is welcome to this project. Pullrequests will be merged!
One further topic here in germany ar the laws, that don't allow driving an electric board on the road. In worst case they can take your car driving license. They are crazy here. That's why I also lost a bit the interest in my electric longboard. It is really sad.

Never the less I have one request to you. I published this peace of software because I wanted to share it with the community. Please don't make it a commercial product. It would be great if you make your case open source and sell it together with a PCB if you want. But please not as a plug and play version.. I hope you can understand me.

Wow. A lot of text. Sorry for. And for sure full of typos. But I'm german. 

I stay tuned for support and to see your progress. Go on!!. 

Andy

PS: The Nunchuck is really nice in handling!
```

---
## \#98 Posted by: RollingGecko Posted at: 2017-05-28T22:42:44.864Z Reads: 286

```
If you want to see it once in action here a video of last years Berlin MakerFaire

[https://www.youtube.com/watch?v=kIexnrNAe1s](https://www.youtube.com/watch?v=kIexnrNAe1s)
```

---
## \#99 Posted by: lox897 Posted at: 2017-05-28T22:48:08.623Z Reads: 286

```
Thanks for the reply @RollingGecko , I believe that an open source case, as well as your code would be a great remote to sell. Of course there would be a donation to you for your amazing work with the project, but if you feel like that is not a good idea, maybe not. There is definitely a market and I think it is too hard for some people here to make it if they dont have a basic knowledge of arduino
```

---
## \#100 Posted by: Mikeomania12 Posted at: 2017-05-29T15:05:20.277Z Reads: 276

```
Yes I agree. Like the vesc is.
```

---
## \#101 Posted by: Print3r Posted at: 2017-05-29T15:28:59.339Z Reads: 281

```
How do you see your screen while riding? It is great that you found this thread! @Sander is working on a new remote that will be similar to yours (with an OLED) but with more features. He is planning to integrate a bluetooth module to the receiver pcb so that you can change max current with a phone, have nice graphs and even display directions on the OLED (Google API), the NRF used will have a PA&LA (to make the signal never cut out) and the receiver will have a current sensor so that the number of watts into the board whilst charging can be calculated. How much did you find you looked at your OLED for stats/ did you just forget about the OLED and use it as a classic wii remote? What projects are you working on (now that eboards are banned in Germany)?
```

---
## \#102 Posted by: RollingGecko Posted at: 2017-05-29T21:09:47.925Z Reads: 282

```
You are right, that the display is a bit covered by the thumb. But if you presss the button to keep the speed over the PID you can look easy to the screen. Then I look often for speed, remaining capacity or the current.
At the moment I'm working on a big 3D printer with 2 individual printheads. I'm looking forward to see @Sanders control. The feature list sounds interesting. To have charging information is interesting. It would also be great to have long time statistics to the battery pack.
Vedders contribution to the community is amazing and a gift. I don't know where he finds the time for. Thank you Vedder. That is why I want to keep also my project open source. So if you developed the hardware put it please also open source as planned. And you are right. Not everybody is willing to enter deep enough is the subject to rebuild a remote. So a plug and play Version would be good.

Regards

Andy
```

---
## \#103 Posted by: lox897 Posted at: 2017-05-29T21:43:25.009Z Reads: 275

```
Of course it would all be open source! I also plan to make detailed videos so if people 3d print the case they can easily buy their own parts and watch the video on assembly. It is time the community had a decent remote :)
```

---
## \#104 Posted by: AndyL Posted at: 2017-06-03T14:11:26.658Z Reads: 286

```
Hey there! Chanced upon this design on thingiverse that resembles the boosted controller alot. I lack the relevant knowledge regarding electronics, so I decided to approach this particular thread for insights. How does this particular remote work using an xbee module? Also, isit possible to use sucha form factor for a vesc controller that you are working on? https://www.thingiverse.com/thing:1602865
```

---
## \#105 Posted by: mptrs Posted at: 2017-06-11T08:26:01.597Z Reads: 271

```
Corrected vote :)
```

---
## \#106 Posted by: lox897 Posted at: 2017-06-11T22:52:19.163Z Reads: 269

```
Little update: all parts are here and I will be making it this weekend
```

---
## \#107 Posted by: kptheinventor Posted at: 2017-06-11T23:04:29.593Z Reads: 269

```
:heart_eyes:
```

---
## \#108 Posted by: Jackyrobb Posted at: 2017-06-13T23:09:27.650Z Reads: 266

```
## Trying to make controller, need help

I'm very excited! I have been trying to use Rolling Gecko's code to a nunchuck controller, but I am having some trouble with the libraries. First off, I'm not quite sure which adafruit library I am supposed to use. It keeps giving me an error about "u8glib" and I have no idea what that is. 

----------

I'm also having trouble understanding **what pins go where**. I noticed you used a 7 pin OLED that has _GND, VCC, D0, D1, RES, DC, and CS_ pins. My OLED has the same pins, but I cannot get mine to work. I'm just not sure where to plug in the oled, potentiometers, or nRF.

 **Please help! Any help would be deeply apreciated!**
```

---
## \#109 Posted by: Jackyrobb Posted at: 2017-06-13T23:10:26.202Z Reads: 262

```
How did you do this?? It's so cool
```

---
## \#110 Posted by: lox897 Posted at: 2017-06-13T23:51:55.525Z Reads: 279

```
[quote="Jackyrobb, post:108, topic:21922"]
I'm very excited! I have been trying to use Rolling Gecko's code to a nunchuck controller, but I am having some trouble with the libraries. First off, I'm not quite sure which adafruit library I am supposed to use. It keeps giving me an error about "u8glib" and I have no idea what that is.
[/quote]

U8G is a library for the display of text and graphics on the OLED display. You will need to download it from here:
https://github.com/olikraus/u8glib

[quote="Jackyrobb, post:108, topic:21922"]
I'm also having trouble understanding what pins go where. I noticed you used a 7 pin OLED that has GND, VCC, D0, D1, RES, DC, and CS pins. My OLED has the same pins, but I cannot get mine to work. I'm just not sure where to plug in the oled, potentiometers, or nRF.
[/quote]
The pinouts are on the config.h file. It is quite simple if you just read through it. I will post a schematic when I get the chance.
```

---
## \#111 Posted by: Jackyrobb Posted at: 2017-06-15T00:33:42.524Z Reads: 274

```
Thanks for the help. I tried going through the config.h but I just couldn't quite get it right. I'm excited to see the schematic!
```

---
## \#112 Posted by: lox897 Posted at: 2017-06-18T02:40:51.264Z Reads: 279

```
@Jackyrobb 
<img src="/uploads/db1493/original/3X/e/d/edc7a9313de66884d078bd8d6f729f4b923a1d9f.png" width="540" height="500">
```

---
## \#113 Posted by: Sander Posted at: 2017-06-18T14:44:58.670Z Reads: 270

```
Why are you not using the CS pin?
```

---
## \#114 Posted by: niktwo17 Posted at: 2017-06-18T18:13:36.333Z Reads: 268

```
So I am right now also working on my own remote using arduinos and nrf24l01.
My code is based on the library from  @RollingGecko 
Im using an sparkle 3D printed case and an potentiometer taken from a broken gt2b
Everything is working fine, but I noticed an odd behavior: 
My motor is actually spinning in the opposite direction compared to PWM mode and the when reading RPM values over UART I get also negative RPM. 
Does someone have an explanation for that or knows how to reverse your board using UART?
Maybe @lox897?
```

---
## \#115 Posted by: lox897 Posted at: 2017-06-18T20:19:11.118Z Reads: 251

```
Not needed
```

---
## \#116 Posted by: lox897 Posted at: 2017-06-18T20:20:38.064Z Reads: 258

```
Does it work fine when you switch two motor cables? Maybe you connected pot wrong way? Or put it in the case the wrong way around?
```

---
## \#117 Posted by: niktwo17 Posted at: 2017-06-18T20:26:59.620Z Reads: 260

```
By using another VESC-UART library it also works normal.
It just seems that ive somehow activated a reverse in this code. I actually dont know how this could be related to my pot.
One direction controls the setcurrent function and the other the setbrake function.
```

---
## \#118 Posted by: lox897 Posted at: 2017-06-18T21:52:25.009Z Reads: 253

```
True! RG was made for a joystick so that could be part of it. How will you switch screens with a potentiometer? Have a look in the transmitter code. I'll have a look tonight once I'm home
```

---
## \#119 Posted by: niktwo17 Posted at: 2017-06-19T20:15:11.605Z Reads: 249

```
Ive had another look but still havent found anything. dont see what could cause this
first this wasnt ment to have a display, i just wanted to use parts from my fried sparkle/gt2b.
but since ive come so far i couldnt resist to order a display. will add prob 2 or 3 switches.
i do definetaly need a way to set my board in some kind of nanny mode as it keeps throwing my friends of :joy:
```

---
## \#120 Posted by: Jackyrobb Posted at: 2017-06-24T14:48:21.288Z Reads: 245

```
Did you finish?
```

---
## \#121 Posted by: lox897 Posted at: 2017-06-25T11:34:44.443Z Reads: 240

```
School holidays now woooooo more time for ESK8. Soldering JST connector tomorrow and will test this week
```

---
## \#122 Posted by: wafflejock Posted at: 2017-06-25T11:56:04.872Z Reads: 255

```
Awesome to see I don't know if I'd seen Rolling Gecko's version yet but I'm sure I've read a lot of their posts before.  I have my own incarnation of a very similar design with PCBs that I made at home.  https://github.com/shusain/eskatecontroller  I considered manufacturing some as well but assembly time and shipping does add to the cost and I have some concerns about FCC in the US since it is a radio transmitter/receiver not sure if I'd really need to get certification (from what I understand can still sell them without it but safer legally if you get it done).  Major issue then is what scale can you make them at where you'll be able to sell your inventory but actually make some sort of profit as well (at least pay for your time).  This is the second post in a couple of hours I've seen with custom remotes also using the same kind of OLED I just got except the one I ordered uses SDA/SCL for communication so just the 2 wire communication which simplifies things.  I haven't settled on what to display on the OLED so hadn't started integrating it with the controller but did some testing with the OLED itself and the adafruit graphics library and it seems to work well so far.
```

---
## \#123 Posted by: lox897 Posted at: 2017-06-25T12:14:47.830Z Reads: 242

```
The I2C displays sure are a lot easier to use. I would like to know why U8Glib was used over the adafruit library, as well as why SPI was used and not I2C. Maybe @RollingGecko could explain these decisions.

Very nice and simple remote! Great job @wafflejock
```

---
## \#124 Posted by: niktwo17 Posted at: 2017-06-25T12:51:38.940Z Reads: 241

```
Maybe because of memory issues?
How much ram does your code use @lox897 
Ive connected a nrf,  0.96 oled, mpu6050, pot and a switch. Im using 85% of my nanos ram and lately it crashes all the time :/
I might go u8 too as it should use less ram than adafruit.
```

---
## \#125 Posted by: wafflejock Posted at: 2017-06-25T12:58:45.219Z Reads: 243

```
If you aren't dynamically allocating memory I don't see how any sort of memory leak could be an issue.  I made a little frogger test app (ported some code from coding train youtube channel) to work using the adafruit library and it seems to run fine but I've only used it for a few minutes at a time really... is the crash time based?  I wonder if it has something to do with power or the actual code.

I have a nrf and arduino mini based transmitter/receiver, I had some issues with a nano being powered off the VESC power but seems fine with the pro mini boards running at 3.3V/8MHz with the VESC power going into the VIN
```

---
## \#126 Posted by: niktwo17 Posted at: 2017-06-25T13:06:59.662Z Reads: 250

```
Well to be more precise, the display is stuck in the initialization screen. So i dont get further than void setup. Other sketches run fine. Only thing ive changed from previous versions is adding  variables
```

---
## \#127 Posted by: Jeefberky Posted at: 2017-06-25T14:37:32.650Z Reads: 274

```
I also made a controller based on the code from rolling gecko. I have a Wii nunchuck laying around and crammed all the stuff inside it.

Inside is an Arduino nano.
The Arduino inside is powered by a spark fun powercell. Which boosts the 1s battery (250mAh) voltage to 5v.

Battery life is good (6+ hours).
Very reliable connection (had no dropouts).
Charging the remote can be done by a micro USB plug that is covered by the Velcro strap.
Using it for almost a year now.

<img src="/uploads/db1493/original/3X/2/7/2739a2f52736c05c939e1a46f7c7f18204edec40.jpg" width="281" height="500">
<img src="/uploads/db1493/original/3X/b/0/b08ad1d809396892752c843fe54f2ef0bba037d4.jpg" width="690" height="388">
```

---
## \#128 Posted by: wafflejock Posted at: 2017-06-25T14:49:31.639Z Reads: 262

```
ah :head_bandage: :hand_splayed: Just remembered I did the adafruit based one on a particle.io photon board so not really a fair comparison or test of it with an arduino.  The Particle.io board is an IoT prototyping platform and uses a similar development environment and compiles C++ for the ARM processor on the board and flashes it over the internet, but has way more resources on that chip compared with an arduino, so maybe an issue there.  Let us know if U8Glib works out better I've only "used" it with the Marlin firmware on my 3D printer and that uses a Mega2560 iirc.
```

---
## \#129 Posted by: wafflejock Posted at: 2017-06-25T14:58:36.387Z Reads: 260

```
Thanks too and yeah I just took the core components from the RC one I was using that I liked or needed and modeled those then stopped :) Went back later and added some stand offs for the PCB to be screwed into as well but it is definitely still pretty simple could use some refining on the design but I've become used to it and fear the change now :smile:
```

---
## \#130 Posted by: RollingGecko Posted at: 2017-06-25T16:08:03.667Z Reads: 268

```
HI,

Up to the problem with the reverted motor:

I don't know if you are using 2 Buttons. I use the button attached to UPPER_BUTTON to switch to revert. If you don't have this attached you will have here a floating state of the pin.  Please give me feedback this can cause the problem. In this case I can toggle this out by config.h. 

Up to the usage of the SPI dispaly. IT was laying around. ;)

To the memory:

The code brings the nano to it's limits. When I compile it, It took also:

Compiling 'ArduBoardControler_TX' for 'Arduino Nano w/ ATmega328'
Program size: 26.754 bytes (used 87% of a 30.720 byte maximum) (2,27 secs)
Minimum Memory Usage: 789 bytes (39% of a 2048 byte maximum)

The code has no dynamic allocated memory. So in runtime there should be no memory issues.

REgards

Andy
```

---
## \#131 Posted by: lox897 Posted at: 2017-06-26T12:24:16.333Z Reads: 258

```
Sweet job. Would you mind posting a pic of the internals?

@RollingGecko As always, much appreciation for your detailed replies and giving back to the community. Final result hopefully tomorrow!!!
```

---
## \#132 Posted by: lox897 Posted at: 2017-07-09T07:21:06.759Z Reads: 241

```
Couldn't find the time to work on it last week and I'm on holiday currently but should be in the shop next week to finish it
```

---
## \#133 Posted by: Jeefberky Posted at: 2017-07-17T20:06:16.090Z Reads: 236

```
I will post pictures in a few days. Don't expect much of it, it is literally crammed in there XD.
```

---
## \#134 Posted by: Pedrodemio Posted at: 2017-07-18T01:49:22.871Z Reads: 259

```
nice work @lox897, I've made a similar remote, but skipped the oled display because lack of space, instead i used the 4 remaining pins to add 4 leds, but never got over implementing any function on them, also, be aware that the C and Z buttons that come with the nunchuck are total crap, my board has some big scratches on the trucks and decks due to the cruise control locking and i had to bail

<img src="/uploads/db1493/original/3X/a/7/a7153904c41a9fd803dacba736b48b9b0339dd21.JPG" width="690" height="460"><img src="/uploads/db1493/original/3X/9/1/914853edb4c7bd64bdbbe5d189ec8bd1ca9021bf.JPG" width="690" height="460"><img src="/uploads/db1493/original/3X/b/d/bd87fcead388d92e0b8d7f96d67a55c42396ca02.JPG" width="690" height="460">
```

---
## \#135 Posted by: wafflejock Posted at: 2017-07-18T02:20:12.645Z Reads: 251

```
Have almost the same exact controller guts but made a 3D printed model and used some seemingly better potentiometers (think they are made for guitars or guitar equipment but they seem solid and give good consistent readings).  With the 5V variant of the arduino running off a single 1S LiPo the signal would be delayed when the battery started to wear down, I switched to 3.3V 8MHz variants that can run at voltages lower than the single lipo cell can run and I got some LiPo cells for quadcopters that have built in low voltage cut off.  Link to github posted above.  Got a small batch of PCBs made to connect the nrf boards and pro mini boards was $28 and some change for 10 of them delivered (only needed 2 so I sent a few pairs to a few other brave souls).
```

---
## \#136 Posted by: lox897 Posted at: 2017-07-31T09:11:44.431Z Reads: 250

```
Sorry for not posting many updates guys! 3D printer is working so here is a photo of it printing. I'll upload the latest design in my hand once the print is done. Need to get the electronics going too but all my soldering gear is behind all the shit in the warehouse! Dammit <img src="/uploads/db1493/original/3X/f/d/fd6b32c025018ea3d2d37d1c5a3c767229d2580d.jpg" width="375" height="500">
```

---
## \#137 Posted by: lox897 Posted at: 2017-07-31T21:31:47.869Z Reads: 256

```
<img src="/uploads/db1493/original/3X/2/0/20d64871ecedeb69e9b42865e2ea047665199ba5.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/b/f/bf16bb3d7b28e578e730f8475f65bf94ddb1b640.jpg" width="375" height="500">
<img src="/uploads/db1493/original/3X/c/4/c440ec32a5ceaf925ab395f88bc8fb3549a00fba.jpg" width="375" height="500">
Need to: Add mounting holes
Find a better system than the joystick since it's too wide (maybe some sort of potentiometer)
Make it thinner and more ergonomic
```

---
## \#138 Posted by: Sander Posted at: 2017-07-31T21:33:52.071Z Reads: 249

```
Nice update, have you been working on any firmware recently?
```

---
## \#139 Posted by: lox897 Posted at: 2017-07-31T21:35:53.177Z Reads: 250

```
No need to. All the RG stuff is ready to go
```

---
## \#140 Posted by: lox897 Posted at: 2017-08-14T03:39:32.814Z Reads: 247

```
Finally got all of my shit out of the warehouse! Time to get high on some solder fumes!!! Will work on the remote soon. PS: iPads have potatoes for cameras, fuck you apple. <img src="/uploads/db1493/original/3X/c/0/c07b75f482ed18ad746cfb0e919e90d023259bf8.jpg" width="375" height="500">
```

---
## \#141 Posted by: ACIN Posted at: 2017-09-03T18:26:09.686Z Reads: 225

```
How is it going?
```

---
## \#142 Posted by: lox897 Posted at: 2017-09-03T20:42:49.928Z Reads: 222

```
Haven't set up all my gear at my house yet. Probably this weekend. Got so much stuff with school no more ESK8 time :frowning:
```

---
## \#143 Posted by: ElskerShadow Posted at: 2017-10-02T21:16:40.761Z Reads: 196

```
No news = good news ?
```

---
## \#144 Posted by: lox897 Posted at: 2017-10-02T21:30:47.511Z Reads: 198

```
On holiday currently. No news = no news
```

---
## \#145 Posted by: ElskerShadow Posted at: 2017-10-02T21:31:51.806Z Reads: 199

```
Well, 
Enjoy your off time !
```

---
## \#146 Posted by: GrecoMan Posted at: 2017-10-03T00:12:35.685Z Reads: 192

```
Lol depending on cost I may buy one in a month or two if there are any left
```

---
## \#147 Posted by: Fabian287 Posted at: 2017-10-31T16:14:25.532Z Reads: 190

```
SPI has a higher refreshrate^^ and does not consume any Analog pins^^
```

---
## \#148 Posted by: Fabian287 Posted at: 2017-10-31T16:24:04.972Z Reads: 200

```
I asked @RollingGecko to implement the support for LIION Batterys for the Nunchuck. Atm i try to help him out^^ (he is trying to implement). I added to the OLED some features for example that u see the drawing watts /Max watts , and that u see the voltage of the remote Lipo.
```

---
## \#149 Posted by: lox897 Posted at: 2017-12-17T07:54:40.191Z Reads: 187

```
After 6 months I’m finally working on this again! From my understanding there are a few other remotes that seem to be finished since this one but I’ll continue to work on this. @RollingGecko there seems to be two issues with the latest version, my display will not work any more and I am getting no response from the joystick. I have also put my VESC settings in the pictures below. Should I be using NRF or UART? I’m guessing I should’ve used UART because it goes through an Arduino first?

Glad to be back on the forum too guys. Should be really active during these 6 weeks of holidays!

<img src="/uploads/db1493/original/3X/5/0/50dccc1adb9d6da7566e563007daaa092c907ee6.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/f/1/f170655c94d8b4a2090c67aadeded58504470d2f.jpeg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/b/cbe82b23c0322736251673d75aded10f92f947fa.jpeg" width="666" height="500">
```

---
## \#150 Posted by: niktwo17 Posted at: 2017-12-17T15:03:01.168Z Reads: 161

```
You need to use UART to communicate between vesc and arduino.
The library for fw 3.x is currently not working correctly. Id suggest you downgrade your vesc firmware to an old version. Then it should work just fine.
```

---
## \#151 Posted by: Der6FingerJo Posted at: 2017-12-17T15:44:03.815Z Reads: 166

```
@RollingGecko made a thread about it: http://www.electric-skateboard.builders/t/tester-needed-for-vescuartcontrol-with-new-interface/38476

Currently VescUartControl is working but ArduBoardControl has some hiccups, maybe you can find a fix! I'm trying to work on this when i finish my own remote project and expand ArduControl a bit.
```

---
## \#152 Posted by: lox897 Posted at: 2017-12-17T20:54:16.391Z Reads: 161

```
Alright, I’m using UART now on a baud rate of 115200 as recommended on that German site that RollingGecko put on his GitHub.

First problem was that all the char variables needed to be changed to const char. That solved about 6 DrawScreen errors for me.

I’m using @Ackmaniac latest firmware. 2.54 or something? Is that a problem?
```

---
## \#153 Posted by: lox897 Posted at: 2017-12-17T21:52:18.406Z Reads: 160

```
So I've worked a bit on the TX, RX, and VESC UART Sample code. Had a few DrawScreen warnings/errors on the TX code which were fixed by changing all the char to const char as mentioned above.

In the RX code I'm still receiving this error in the Arduino IDE:
> /Users/myusername/Desktop/ArduBoardControler-master/ArduBoardControler_Rx/ArduBoardControler_Rx.ino: In function 'void loop()':
> /Users/myusername/Desktop/ArduBoardControler-master/ArduBoardControler_Rx/ArduBoardControler_Rx.ino:100:77: warning: large integer implicitly truncated to unsigned type [-Woverflow]
> radio.writeAckPayload(pipe, &VescMeasuredValues, sizeof(VescMeasuredValues));

I believe this is because we are truncating a type that doesn't have enough bytes or storage or something to a lower type? Could this also muck up the values?

The third error which I fixed for VESC UART Sample was the vescuart.cpp script in the VESC UART Control library which set a value to NULL and was ignored by replacing NULL with a 0.

I'm no programmer (this is just me with a bit of google work) so I don't think these are big changes and may even be the wrong changes but they certainly have eliminated some errors.
```

---
## \#154 Posted by: lox897 Posted at: 2017-12-17T22:47:12.156Z Reads: 168

```
Now onto working with the example in the VESC UART Control library. I'm having issues with communicating with the VESC. Both baud rates are on 115200 and I'm using the serial monitor but I'm getting a failed to read data error.

Here's the code for the VESC UART Sample:
> // the setup function runs once when you press reset or power the board
> // To use VescUartControl stand alone you need to define a config.h file, that should contain the Serial or you have to comment the line
> // #include Config.h out in VescUart.h

> //Include libraries copied from VESC
> #include "VescUart.h"
> #include "datatypes.h"


> #define DEBUG
> unsigned long count;

> void setup() {
> 	
> 	//Setup UART port
> 	Serial1.begin(115200);
> #ifdef DEBUG
> 	//SEtup debug port
> 	Serial.begin(115200);
> 	#endif
> }

> struct bldcMeasure measuredValues;
> 	
> // the loop function runs over and over again until power down or reset
> void loop() {
> 	//int len=0;
> 	//len = ReceiveUartMessage(message);
> 	//if (len > 0)
> 	//{
> 	//	len = PackSendPayload(message, len);
> 	//	len = 0;
> 	//}
> 	
> 	if (VescUartGetValue(measuredValues)) {
> 		Serial.print("Loop: "); Serial.println(count++);
> 		SerialPrint(measuredValues);
> 	}
> 	else
> 	{
> 		Serial.println("Failed to get data!");
> 	}
> 	
> }

So I tried uncommenting #include "Config.h" out in VescUart.h and then I get an error saying unable to find Config.h. Tried again this time but did a path directly to Config.h and still got errors.

In the VESC UART Sample script it tells me that Serial1.begin is undefined.
Then I tried to include Config.h in the VESC UART Sample script and still got an undefined error.

@RollingGecko what do you think the problem could be here?

@Der6FingerJo I believe you had success with this on a later firmware of VESC. Maybe I'm using the wrong VESC UART library?
```

---
## \#155 Posted by: Der6FingerJo Posted at: 2017-12-17T22:59:14.391Z Reads: 158

```
There are 2 versions of VescUartControl right now, one for older firmwares and one for 3.xx firmware. You can find the new one as a branch on GitHub. I had success using the new one (called Vesc 6) on an Arduino Mega with 3.xx firmware without modifying anything in the example sketch.
```

---
## \#156 Posted by: lox897 Posted at: 2017-12-17T23:35:38.239Z Reads: 162

```
I’m using an Arduino Nano. That may be where the problem lies. So for my 2.54 firmware VESC should I be using 0.1.5 or Master @RollingGecko ?

I’m happy to help solve the nano problems if you can direct me to the next step from here.
```

---
## \#157 Posted by: lox897 Posted at: 2018-04-07T03:30:51.664Z Reads: 117

```
@RollingGecko how's it all going? Have there been some bug fixes?
```

---
