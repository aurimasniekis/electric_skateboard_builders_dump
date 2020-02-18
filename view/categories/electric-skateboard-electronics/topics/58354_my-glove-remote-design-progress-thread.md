# My Glove Remote Design+Progress Thread

### Replies: 45 Views: 1344

## \#1 Posted by: faithfulpuppy Posted at: 2018-06-09T20:52:08.765Z Reads: 402

```
Some of you may have seen @InitialDriveGTR 's  flex-sensor based glove controller. The funny thing is, while he was ordering parts for his, I was also gathering parts for mine. I didn't copy his design and he didn't copy mine obviously, we both came up with the same thing at the same time.

That being said, he's way more experienced with arduinos and designing these types of systems and the like, so I'll definitely be taking some cues from his design

anyway, I finally got some time this weekend (schoolyear almost over!) to start designing my own version of the esk8 glove controller. I don't wanna crack open my esk8 so I grabbed my quadcopter to use for testing. I'm posting the video (and the code, screenshots, and schematics) below.

tell me what you guys think, or any ideas for improving it as usual

-Joe
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2018-06-09T20:56:26.497Z Reads: 391

```
https://www.youtube.com/watch?v=K4v2qZm7Ghc


First test: it's a little jumpy as far as how it gets started, but i think i could code a function that ramps the pwm values up and down more gradually. I've also tried putting a 10uF capacitor in parallel with the flex sensor but it seemed to pull the voltage down over time, instead of remaining constant when left alone
```

---
## \#3 Posted by: faithfulpuppy Posted at: 2018-06-09T20:57:46.463Z Reads: 372

```
also: the reason it's cutting out near the top rpm is becase the function that generates the pwm value is going over 255, which is the maximum that the pwm function takes, if that makes sense. I have very little coding experience so idk if i'm using the right terminology
```

---
## \#4 Posted by: faithfulpuppy Posted at: 2018-06-09T21:08:07.998Z Reads: 354

```
![image|375x500](upload://8rRoQnGvPKQGAiGsRuWAR8cZahK.jpg)

here's an overhead shot of the breadboard so you can see exactly how it's set up. Nothing too complicated, just messy because I'm a total noob. the resistor is 100KOhm
```

---
## \#5 Posted by: plasteroid Posted at: 2018-06-09T21:40:49.677Z Reads: 327

```
Looks like a really cool idea.   

So if I understand correctly, you are going to attach that flexy piece to a glove to act as your trigger finger?
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2018-06-10T02:31:22.059Z Reads: 294

```
yeah, exactly. Probably multiple if i can figure out how to use that for more precision, such as one on my first finger for throttle and one on the pinky for braking
```

---
## \#7 Posted by: Scoo_B_SK8 Posted at: 2018-06-10T03:52:07.305Z Reads: 289

```
I believe you might want to use “constrain” for min and max value (0-255).
https://www.arduino.cc/reference/en/language/functions/math/constrain/

I also have messed with this design.  Safety things to consider...
•away to engage/disengage the use of the throttle (ie when not on board or on board when you dont want any type of action to take place) 
•fingers will change position when trying to balance out of a situation.
•brakes, dont want them to start braking at an unwanted time either 😬

Possible solutions...
• pressure sensor / built in switch(tactile button)
• using multiple flex resistors for throttle 
• tactile button + flex resistor 

Main issue is safety “checks and balances” as to not get tossed from your board from sudden acceleration/burst or jumps of or brakes suddenly engaging.

Not trying to discourage you at all.  Id love to see what you come up with.
```

---
## \#8 Posted by: faithfulpuppy Posted at: 2018-06-10T15:19:52.380Z Reads: 256

```
thank you, this is exactly the kind of feedback i was hoping for!
* i think i'll have  a dead man's switch somewhere on the glove, or a small slide switch that turns off throttle control without turning off the glove
* I hadn't thought of that, I'm gonna need to work around it and test a bunch of different solutions to see if it works
* i want to put brake controls on my pinky, so two different fingers are involved in the overall throttle control

I'm going to need a lot of different things going on here to prevent injury, but i think the most important thing is that the fail state should either be neutral or a very gentle brake
```

---
## \#9 Posted by: faithfulpuppy Posted at: 2018-06-10T15:20:52.020Z Reads: 253

```
here's test two: now glove-mounted!
https://www.youtube.com/watch?v=LZ5mfsSAMPE
```

---
## \#10 Posted by: DevinG Posted at: 2018-06-10T15:26:04.490Z Reads: 242

```
Awesome R&D watchin this! :eye:
```

---
## \#11 Posted by: sunnyD Posted at: 2018-06-10T16:27:40.169Z Reads: 229

```
oh this is soooooo frikin cool. I would buy one rn XD
```

---
## \#12 Posted by: faithfulpuppy Posted at: 2018-06-10T20:24:21.963Z Reads: 211

```
maybe if i get this working really well, i might consider selling. That being said, it's pretty simple to make yourself
```

---
## \#13 Posted by: sunnyD Posted at: 2018-06-10T20:26:23.568Z Reads: 212

```
haha, im in no sense handy with this kind of thing, there is a reason i'm not studying for a major in engineering. So if you do start making these, ill take nine :wink:
```

---
## \#14 Posted by: Blitz Posted at: 2018-06-10T22:08:23.602Z Reads: 202

```
Would this Glove remote work for someone with arthritis? (Scenario) Pulls finger for Gas Oh no It's stuck oh no not again...phew it was just a dream.
```

---
## \#15 Posted by: faithfulpuppy Posted at: 2018-06-10T23:01:49.180Z Reads: 198

```
i don't know that any of our esk8 equipment works that well for people with arthritis
```

---
## \#16 Posted by: faithfulpuppy Posted at: 2018-06-11T01:50:13.253Z Reads: 201

```
Last update for tonight. Just got a second sensor wired up and coded it in. I don't know exactly how I'm gonna handle the two different inputs (should I add them, subtract them, average them? I have no idea) but I'll have a few days to think about it before I get back to work. One more day of school, then two days of tests.

![IMG_20180610_202644|375x500](upload://igX2l7djk19PnwF9UdkkBuRBRYD.jpg)
```

---
## \#17 Posted by: InitialDriveGTR Posted at: 2018-06-14T02:06:24.230Z Reads: 188

```
I'm assuming you're operating your circuit as a voltage divider, fed into the ADC. I'd bet money you found that the digital value you are getting is operating within a range, and not between 0 and 255 (8bit) or 0 and 1023 (10bit). Of course you can identify your operating range and scale it to fit your output (PWM) which from what I read is 0 - 255. That will linearly sync your measured resistance from fully relaxed to fully flexed to your ESC output. 

The downside to using this method is that since you are effectively "zooming" in on a small section of your ADCs measurable range (0v to 5v in the case of your Nano there **RIP my two, I fried them two days ago and was forced to change platforms**), your output will become very jumpy due to insufficient resolution on your input.

I haven't looked into the ADC on the Nano very much to see if it even has this, but the proper way to handle a voltage divider based input is to have an ADC with +VRef and -VRef inputs. 

On an integrated board such as the Nano, this would mean using up an additional two analog inputs to be used as your VRef inputs, however you would be able to take two trimmer pots (one for the +VRef and the other for the -VRef) and then the ADC channel actually reading the flex sensor, will only measure the voltage range you want. 

There are ways to do this completely by potentiometer but its a shitload of tweaking, it's not very reliable, and there are other drawbacks such as excess power consumption. The E-INK displays I'm using on my design have to be driven with RAM restrictions on the 328 AVRs. I just got two ESP8366's in today that have only one analog input and that means I can't directly use one on the glove side of the LCS. Since I'm using SPI as my main communication bus for the radio and display, I figured why not use a 4ch 12bit SPI chip...

![Screenshot_20180613-215054_Drive|243x500](upload://qk1NeNSEqt1nMI8hR7LS1vfhYHT.jpg)

Hope this helps you tackle some of the problems I think you may encounter... I have about 20 years of experience building electronic systems ;P so let me know if you need any guidance, I'd be more than happy to help. Two people tackling the same problem is still a 100% increase in efficiency overall. 

![20180613_232408|690x452](upload://2d62tQ6WoH8rUknbOE9Kq6J4Qia.jpg)
```

---
## \#18 Posted by: Scoo_B_SK8 Posted at: 2018-06-14T04:33:49.017Z Reads: 166

```
#1 that work space = mad scientist at play :wink:

#2 id look into this guy here "gy-ads1115/ads1015" i use them with ESP8266's for automation sensors and is all package up in a breakout board.  4ch, Comparative, gain amplifier, I2C, voltage 2.0v-5.5v, addressable up to 4 on a single I2C line.

@InitialDriveGTR ... what is the advantage/(your plan) of using ESP8266 vs. NANO or PRO-MINI on the glove remote?
 
![gy-ads1115_ads1015|666x500](upload://lGWvf34NNP0YDqAzuilwToiWk3D.jpg) 

i had crossed this idea a while back with other users but safety checks and balances stopped me from pursuing this and put the project in park till came up with some... and well other projects just took its place, so I'm happy to see the both of you working on this project and am excited to see what you all come up with and maybe "lend a hand" when i can and maybe follow along with a 3rd prototype (since already have all the electronic parts already) as to have extra data numbers/input differences that may arise for tuning the end product.
```

---
## \#19 Posted by: InitialDriveGTR Posted at: 2018-06-14T04:43:47.893Z Reads: 146

```
I saw those ADCs but I ordered the 3204s on my business mouser account ;) I can can also run them at a way higher speed than I2C on HSPI...

I switched to the ESP primarily because with the nano, I have to load graphics into RAM in chunks and send them to the display in sequential packages to build the graphic THEN push the image onto the actual display. Wifh the ESP, I have enough RAM to load a graphic from flash, send, and display all in one shot. All glove related DSP will handled on the glove side of the interface to minimize overhead on the RF link.
```

---
## \#20 Posted by: faithfulpuppy Posted at: 2018-06-14T05:02:19.938Z Reads: 153

```
thank you, this is exactly the kind of technical response i was hoping for!

yeah, that's exactly what's been happening so far. i've successfully scaled and mapped the main throttle (i'm only reading from two fingers) but the second one is just returning a weird oscillation that almost looks like it's reading the pwm output or something. weird.

I wanted to use a voltage divider because i want my final design to be as simple as possible and i planned on replacing the arduino with an ATTiny45, but it looks like my code is gonna end up being too large for its 4KB capacity. c'est la vie i guess.

your response does have some stuff in it I don't understand (again, highschooler with no real experience in coding or electrical engineering) but that's perfect because it gives me something to read about in the next few days.

I'm getting really excited about this project, loving all your updates bro
```

---
## \#21 Posted by: InitialDriveGTR Posted at: 2018-06-14T05:51:15.532Z Reads: 135

```
Lol hey I'm self taught through trial, error and forums like these. 

The wierd oscillation could be several things. When I started testing my sensors it was immediately obvious securing the sensor at more than one point on the hand does some funky stuff. I have my sensors secured behind my knuckles, the rest of the sensor is free to move along your fingers and I get very stable and linear feedback even without adjusting for VRef and with 5% shitty 80's resistors. 

Make sure all your grounds are going to a single point, ground loops can do some wierd stuff. 

Put a 10uF electrolytic cap on you VIN, 3.3v and 5v rails and that should clear up most noise being generated by the ESC.
```

---
## \#22 Posted by: pat.speed Posted at: 2018-06-14T06:06:28.955Z Reads: 142

```
damn, I had this exact idea a few months ago and started looking into the process, but I didn't get much further as I'm a student and haven't got much money to throw into things that may or may not work. 

I love how this is going and once you guarantee that it's working I might have a crack at my own version, just have to get good with Arduino coding first.

I'm guessing you will send the code through nrf modules? that would help as you might be able to reuse some of @RollingGecko's code. Oh and I suggest a dead man's switch just incase you get a cramp or something.

Good luck and I'm definitely watching this.

Edit: I just looked up and you already talked about using a dead man switch
```

---
## \#23 Posted by: faithfulpuppy Posted at: 2018-06-14T22:26:10.517Z Reads: 153

```
I'm working off of a greatscott video (that's how i got started on this whole mess of a journey two years ago lmao) as far as my electronics, but the code I'm doing from scratch because it's fairly simple.

anyway, update time. Here's a video of the issue i've been dealing with:
https://www.youtube.com/watch?v=1R97MdJf7G4

the problem is basically shown by 1:10. As I said in the video, both sensors are hooked up exactly the same way and are read by essentially the same code.
![Screenshot%20(41)|413x499](upload://yqQuVFIxKk7NJO1KxPJ43KMxdqv.png)

any ideas on what i'm doing wrong? it's acting like the resistor i have in series with the sensor just isn't there or something but my multimeter reads it to be around 100kOhm
```

---
## \#24 Posted by: faithfulpuppy Posted at: 2018-06-14T22:32:03.914Z Reads: 126

```
ok, i've narrowed it down to the flex sensor itself. I don't think any current is getting through it. I don't know how it took until now to catch this.
```

---
## \#25 Posted by: Scoo_B_SK8 Posted at: 2018-06-15T00:25:50.056Z Reads: 126

```
are you able to swap flex sensors to see if same result?  DBL check wiring  <== usually what happens to me is i miss the row on the breadboard im aiming for.
```

---
## \#26 Posted by: faithfulpuppy Posted at: 2018-06-15T00:29:36.769Z Reads: 120

```
Yeah I swapped them and it seems the flex sensor itself was the problem, and the reason I didn't catch it earlier was because my wiring was wrong
```

---
## \#27 Posted by: faithfulpuppy Posted at: 2018-06-15T01:53:50.534Z Reads: 126

```
ok. I think i know what i did wrong. I burned the flex sensor when i soldered it, making its resistance super high. I did it again on the third one but i figured it out and got my fourth (and final!) one soldered correctly. Good thing i ordered more than i needed! now i need to figure out the algorithm for combining both inputs, and i think i'm gonna run it through the EMA thing on [this article](https://www.norwegiancreations.com/2016/01/tutorial-multiple-values-in-the-arduino-ide-serial-plotter/) to smooth it out a little.
```

---
## \#28 Posted by: InitialDriveGTR Posted at: 2018-06-15T03:11:27.785Z Reads: 126

```
Gah I just saw this now. You have to be super fast soldering to the flex sensor pins. A solid alternate to connecting them is by removing the plastic casing from a female jumper wire, 1/16" heatshrink .5" up the wire jacket to the end of the pin. Make two, stick on the sensor then 3/8" heatshrink it together after placing a dab of hot glue in the middle. That joint will not fail you.
```

---
## \#29 Posted by: pat.speed Posted at: 2018-06-15T03:26:41.797Z Reads: 124

```
Were you able to find a good source of the flex sensors, the cheapest I could find was about $20
```

---
## \#30 Posted by: Scoo_B_SK8 Posted at: 2018-06-15T03:31:06.464Z Reads: 128

```
@pat.speed I got mine from store (Micro enter) $8.99 "Adafruit Short Flex/Bend Sensor"

Also have "AdaFruit Force-sensitive Resistor"... same store $6.99
```

---
## \#31 Posted by: faithfulpuppy Posted at: 2018-06-15T03:47:34.492Z Reads: 117

```
yeah these were the only ones i was able to get. There are the short ones (the ones i'm using) and the long ones (the $20 ones which are better)
```

---
## \#32 Posted by: InitialDriveGTR Posted at: 2018-06-15T04:33:14.689Z Reads: 116

```
I looked at your code. What are you using for resistor values on your divider circuit? Are you using D2 as your high side on the divider circuit?
```

---
## \#33 Posted by: faithfulpuppy Posted at: 2018-06-15T05:48:24.830Z Reads: 108

```
1) about 100kohm. They're super ghetto and not at all within tolerances but they work ok
2) yeah, is there a better way to do that?
```

---
## \#34 Posted by: InitialDriveGTR Posted at: 2018-06-15T13:50:30.422Z Reads: 110

```
You should never use a digital pin as a power source for analog sensors. You are relying on the internal silicon circuits that are used for everything else inside the 328 and this is the best place to get noise on your sensor circuit. It may seem efficient to be able to turn the divider on or off, but at 5V, 120,000 ohms will only draw 0.000041A and thats negligible current draw in this application. 

The nanos are 5v, so your positive voltage supply to the divider needs to be tied to the 5V rail (5V pin). 

100k is too high. The flex sensors are about 20k - 10k, and if you put them in with 100k resistors you will only be able to read about 20% of the full range on the ADC.

Swapping the 100k for 10k should open up your bandwidth a lot.
```

---
## \#35 Posted by: faithfulpuppy Posted at: 2018-06-15T17:34:30.608Z Reads: 106

```
i checked my flex sensors with my multimeter and they actually range from about 35 to 70k, but see if i can swap it to something closer. Switching my voltage supply is a good tip though, and it should knock off a few bytes of code for the attiny
```

---
## \#36 Posted by: banjaxxed Posted at: 2018-07-16T12:04:07.054Z Reads: 103

```
I've been watching the glove tech coming along from yourself & @InitialDriveGTR things are looking to come together, so congrats to you both.

I had a question regarding fingers gesture being the control method, had either of you considered proximity sensors or are they too unreliable?

You know, the sensor is on the deck mounted on truck holes, the glove has a small cicuit sown in and you reach out to the front truck to accelerate (throttling up) & pull glove back to throttle down, it the toerances are right then the speed stance could favor it?
```

---
## \#37 Posted by: DeathCookies Posted at: 2018-07-16T13:52:19.249Z Reads: 98

```
I am still curious what will happen if you Fall.
You want to absorb the landing with your hands and the Board gets wrong or Bad input. 
Carvons Board just got totally crashed by wrong input in just a couple of seconds.. 
What happens if your hand got hit by a stone or something else (falling fruits, insects,...) and you make a wrong Hand movement because of the pain / Reflex ? 

If you make a Low responding Filter you wont Fall  with a wrong Hand movement but you loose the ability to respond quickly for obstacles...

In my mind this controll Mode is too risky. Maybe i do not See the better Plan behind it?
```

---
## \#38 Posted by: InitialDriveGTR Posted at: 2018-07-16T13:58:46.202Z Reads: 101

```
Not a bad idea, but if you used that method, at the distance between your hand and the proximity sensor, the sensor would also detect anything and everything with a magnetic field that you pass by...
```

---
## \#39 Posted by: banjaxxed Posted at: 2018-07-16T14:16:55.652Z Reads: 100

```
That's very true, I was thinking more around a proximity chip system but not sure of the tech

IR maybes?
http://qqtrading.com.my/infrared-proximity-sensor-10-80cm-sharp-gp2y0a21yk0f
```

---
## \#40 Posted by: faithfulpuppy Posted at: 2018-07-17T22:03:04.855Z Reads: 80

```
sorry for the lack of updates, i left NYC (summer break wooo!!!!) and i won't be back for a couple more weeks. I am free to dick around on here though ;)

I hadn't considered a proximity sensor, i was going off the flex thing because i wanted to mimic the motion you make when you're actually using a trigger-style controller. I think the proximity sensor could work, but i'd be worried about having to make a full-body movement to adjust throttle.
```

---
## \#41 Posted by: InitialDriveGTR Posted at: 2018-07-20T00:42:18.510Z Reads: 68

```
All the close proximity data systems I'm aware of ie NFC, RFID etc. all only work at less than a foot. Additionally, in terms of the sensor/antenna that detects whatever, its not possible to detect distance or signal strength, all you will be able to do is detect connected or not connect. I personally dislike the idea of my throttle jumping from 0 to 100%...
```

---
## \#42 Posted by: faithfulpuppy Posted at: 2018-07-20T17:51:59.701Z Reads: 61

```
ah, good point. Either way, im gonna stick to developing with the flex sensors because I'm having enough trouble just with those
```

---
## \#43 Posted by: faithfulpuppy Posted at: 2018-07-21T14:20:38.707Z Reads: 58

```
as a side note, this project has really piqued my interest in electrical engineering. can anyone recommend some good learning material (books, lectures, youtube videos) i can watch to fundamentally understand EE? It's one of the majors I'm considering for college.
```

---
## \#44 Posted by: faithfulpuppy Posted at: 2018-12-18T17:35:44.398Z Reads: 40

```
I've been MIA from this forum since the school year started, wow a lot has changed while I was gone. I wanna get back on this project soon now that I know where I'm going to college, so I'll try to have some updates in january or february. Consider this my note-to-self.
```

---
## \#45 Posted by: totalgeek9224 Posted at: 2018-12-18T18:01:43.497Z Reads: 39

```
![Thanks%20completely%20flew%20over%20my%20head%20pic%20related%20its%20_f6313a873a7fb79b0021cf2f88bf6388|425x404](upload://mQ0tODs6xHSkQOiwkz8OFRfXuQO.png) 
https://media.giphy.com/media/8iEddA9f5wD72/giphy.gif
```

---
