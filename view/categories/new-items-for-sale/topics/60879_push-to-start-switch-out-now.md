# Push to start switch \[OUT NOW!\]

### Replies: 283 Views: 10438

## \#1 Posted by: Martinsp Posted at: 2018-07-04T13:40:57.859Z Reads: 1237

```
Hello everyone,

I was designing and prototyping this kind of a switch for some time now. I finally have a working design and prototype.

![2|500x500](upload://cfsHS3Is4a8ire8vEVGZcP3CM2F.jpg)

The basic operation will be that you just connect this between your battery/BMS and your ESC. Two small wires to your motor phases (I will provide a tutorial) on your VESC (or other ESC) or on your connectors, depending on what is easier for you. 
Now you can just push off on your board once and the power will turn on. It will be in complete OFF state just like any other power switch out there today so it will not drain your battery if you dont disconnect it (Of course it takes some current for the motor rotation sensing but it is very small).
Connecting a regular pushbutton or even a momentary switch will be possible if you would like to for example disabled the push to start feature. The switch has a small MCU on board so we could even set up the push to start feature in such a way that to turn the board off, user interaction would be necessary to prevent the board from turning off unintentionally.

Now I am trying to figure out some things and that is where your feedback and ideas come in. Since I am designing this from the ground up I would like to know what you think and make this as great as it can be :) 

My question right now is, how much time would you like the board to remain ON after the motor stops rotating/you stop riding?

http://electricskateboard.repair/index.php?id_product=41&controller=product 
I will update the product page with images and such ASAP.
Martin.
```

---
## \#2 Posted by: Silverline Posted at: 2018-07-04T13:44:09.626Z Reads: 1041

```
I dont understand. Does it also turn off by itself ?
```

---
## \#3 Posted by: Martinsp Posted at: 2018-07-04T13:45:52.848Z Reads: 1023

```
Yes, it does. When the board is off you can just step on your board, push off (like on a regular longboard/skateboard) and that will turn the board ON.
```

---
## \#4 Posted by: Deckoz Posted at: 2018-07-04T13:51:17.954Z Reads: 1015

```
I suggest not having auto turn off, and just clamping to on state with the bemf voltage, and have a momentary switch for turning off.
```

---
## \#5 Posted by: Martinsp Posted at: 2018-07-04T13:51:58.889Z Reads: 987

```
I forgot to mention that there will be an option to connect a pushbutton, thank you for reminding me I will edit it.
```

---
## \#6 Posted by: Deckoz Posted at: 2018-07-04T13:56:57.091Z Reads: 958

```
Sure, thing. But 

[quote="Martinsp, post:1, topic:60879"]
My question right now is, how much time would you like the board to remain ON after the motor stops rotating/you stop riding?
[/quote]

This shouldn't even be programmed in, mechanical unlatching via push button ONLY. As any type of auto-off is a safety concern if you are specifically using BEMF voltage as your data source.

THE ONLY way I would include an auto off is if your device was also a UART device of the VESC, and measuring eRPM telemetry. 

This should be cool, but please take my suggestion for auto off seriously, I'm sure you can find many of my view points on safety. ;)
```

---
## \#7 Posted by: Martinsp Posted at: 2018-07-04T14:00:37.218Z Reads: 895

```
Safety is definitely up there as a priority!

The switch will be sensing motor rotation so I think that as long as the motor is rotating (under power or just rolling down hill) the switch should not turn off, after the motor stops the switch could turn off after say 5 minutes or so.

I know that some of the ESCs out there have such a feature, does anyone know how the turning off is done there? I have not used one of those yet myself.
```

---
## \#9 Posted by: Martinsp Posted at: 2018-07-04T14:12:38.966Z Reads: 815

```
The switch will not be prompting the VESC to boot via UART or anything like that, that would need some stand by current which is something I tried to avoid. The switch will sense the motor rotation from two of the phase wires and will keep everything connected after the switch (ESCs, lights etc.) completely off. It will turn on as if you pushed a button on a regular switch once the motor starts rotating and generates voltage on the coils/phase wires.
```

---
## \#10 Posted by: BooYA Posted at: 2018-07-04T14:24:16.339Z Reads: 771

```
I think this idea is great, and actually way safer than traditional push-button as it means the board will always be forced ON whenever running. In case the board turns OFF while waiting at a red light in traffic, you would just need to push to start, way faster than having to find your push-button and start accelerating! 
Also why would you need a MCU? It should be possible to activate the FETs using bemf of the motor... And using some caps to act as a time delay to turn the board off.
```

---
## \#11 Posted by: Martinsp Posted at: 2018-07-04T14:27:18.358Z Reads: 721

```
Thank you, yes that would be possible. I thought of just using comparator to sense the rotation. But using an MCU gives me/us more freedom in terms of what we can do.
```

---
## \#12 Posted by: linsus Posted at: 2018-07-04T15:03:06.551Z Reads: 682

```
Put a buck converter for 12V in there as well while you're at it. 😏
```

---
## \#13 Posted by: Martinsp Posted at: 2018-07-04T15:05:48.020Z Reads: 662

```
I feel like that is not the best way to go. I think that not a lot of people would use it but everyone would have to pay for it since it would increase the price. I think that using a stand alone module if you need 12V output is a better option, sorry.
```

---
## \#14 Posted by: mikenyc Posted at: 2018-07-04T15:11:13.526Z Reads: 671

```
[quote="BooYA, post:10, topic:60879"]
In case the board turns OFF while waiting at a red light in traffic, you would just need to push to start, way faster than having to find your push-button and start accelerating!
[/quote]

Interesting use case. If the board shuts off and then turns back on, you’ll have to wait a few seconds for the remote to rebind. Not a terrible scenario when you know the board is off and you're starting it up, but can be annoyingly awkward when you think it's still on, start pushing and there's no response from the remote, or the throttle kicks in at a level that you're not expecting it to.
```

---
## \#15 Posted by: Martinsp Posted at: 2018-07-04T15:15:38.563Z Reads: 635

```
That is true, that is partially why I agree that turning the board off will require user intervention is a pretty good idea. After all, when you want to turn the board off it is not that big of a deal to reach down and press a button. But being able to just push off on the board to turn it on is a useful feature.
```

---
## \#16 Posted by: BooYA Posted at: 2018-07-04T15:16:34.415Z Reads: 623

```
Yeah I get your point, for some remotes can be annoying... But with my dual focbox gt2b, takes about 1second for the whole system to start /bind
```

---
## \#17 Posted by: Sender Posted at: 2018-07-04T15:37:08.024Z Reads: 619

```
I am with @Deckoz on this. No automatic off.  I am in city riding where there are definitely scenarios where I am still for a couple minutes.  Like @mikenyc said, it would be annoying/confusing delay with the remote .  

Also if using a nano x, you are now uncaliberated.... bad things could happen.
```

---
## \#18 Posted by: Battosaii Posted at: 2018-07-04T15:41:23.611Z Reads: 608

```
I'd like to try it. I want least amount of stuff on my enclosure as possible. If possible I'd like just a charge port.
```

---
## \#19 Posted by: Jc06505n Posted at: 2018-07-04T15:45:03.276Z Reads: 603

```
Maybe a minimum limit of 10 mins? If your standing completely still for more than 7 mins, especially in the city , you might as well pick up your Board and walk .

Edit: or maybe 30? That way it simply acts like a 2nd measure to ensure that the board isn’t on all night
```

---
## \#20 Posted by: Sender Posted at: 2018-07-04T15:49:34.390Z Reads: 595

```
Yeah, if it is present at all it should be a longer amount of time than a ridiculously long red light.  But imagine using a nano x (one of the most common remotes).

If there is only the automatic off and not a switch for the "fully off" you would have to wait for your board to power off again, then calibrate your nano x, then push start to go again..... sounds.... irritating to say the least.
```

---
## \#21 Posted by: Martinsp Posted at: 2018-07-04T15:56:05.122Z Reads: 534

```
Okay so the way I see it now, I added a trim pot to the PCB as well as jumper pads to choose if you want to use a pushbutton too or not. So each user will be able to switch back and forth depending on what you prefer as well as choosing the amount of time it takes to turn off.

EDIT: Maybe from 10 minutes upwards to say 45?
```

---
## \#22 Posted by: Deckoz Posted at: 2018-07-04T16:05:53.775Z Reads: 518

```
[quote="Sender, post:20, topic:60879"]
then calibrate your nano x, then push start to go again… sounds… irritating to say the least
[/quote]

Can just pick up your powered wheels and go full brake, then full throttle, set it back down, good to go ;)

No power cycle required
```

---
## \#23 Posted by: ElskerShadow Posted at: 2018-07-04T16:09:56.653Z Reads: 501

```
[quote="Martinsp, post:1, topic:60879"]
My question right now is, how much time would you like the board to remain ON after the motor stops rotating/you stop riding?
[/quote]

The sweet spot would be 5-10 mins, more is kinda useless
```

---
## \#24 Posted by: wafflejock Posted at: 2018-07-04T16:20:24.803Z Reads: 495

```
Why do you want auto off? I don't really understand the use of it.  I've accidentally left my board on overnight more than once and never find that it drains much power.  A few posts in the thread here say it consumes about 20-25mA when just idle https://vesc-project.com/node/222 the arm processors are generally designed to be low power consumption so as long as the control signal is idle the board shouldn't be using any significant power.

Pretty sure my lights consume more power but they have their own battery in my case, guess it would be useful for turning off extra electronics outside the vesc.
```

---
## \#25 Posted by: Martinsp Posted at: 2018-07-04T16:23:21.605Z Reads: 464

```
Depending on the size of your battery you may be in trouble if you have your discharged board on over night you may drop the voltage too low even though the board consumes 20mA or so. The discharge curve under 3V per cell is pretty steep
```

---
## \#26 Posted by: Jc06505n Posted at: 2018-07-04T16:24:20.692Z Reads: 473

```
Was this tested with a Bluetooth module attached and connected?  

I believe (could be wrong) Inboard users would run into an issue where their board would be dead - near dead the next morning bye to the board always searching for a connection

Plus the last thing I want Is to accidentally leave my board on all night , grab my remote and have a whole on the wall cause I forgot to turn it off.
```

---
## \#27 Posted by: wafflejock Posted at: 2018-07-04T16:26:47.108Z Reads: 459

```
Okay I guess I can understand that, I typically will at least partially recharge if I know my batteries are really low when I get home but I also have high cut offs so things aren't likely to go over the cliff.  In that case though can easily have the cut off at like 30m-1h and have it never be an issue while someone is riding.
```

---
## \#28 Posted by: wafflejock Posted at: 2018-07-04T16:35:27.642Z Reads: 453

```
Some sort of audible signal would be good too, I'm not entirely sure the complexity added with a piezo speaker but would be nice if it gave some sort of alert before auto shut off.  Alternatively could have a mode for alarm only vs alarm and auto shutoff.  Maybe use dip switches for configuration since getting the pot position correct and to stay stable might be an issue.

The alarm would be nice in case something disconnects on the sense cables or that logic otherwise fails and at least let's you know it's about to cut out.
```

---
## \#29 Posted by: Sender Posted at: 2018-07-04T17:04:35.547Z Reads: 417

```
Yeah good point, but it would still suck


BTW, happy 4th guys!
```

---
## \#30 Posted by: sunnyD Posted at: 2018-07-04T17:29:49.083Z Reads: 425

```
I understand my opinion is not incredibly educated and probably not the voice of reason but i think a good 5 minutes after having it not move it should turn off. 1. you almost never spend 5min at a traffic light. 2. in my experience i've never waited while actively riding for more than 3ish minutes. Also maybe allow people who the what tf their doing with programming to easily change that time.
```

---
## \#31 Posted by: Kug3lis Posted at: 2018-07-04T18:10:57.934Z Reads: 404

```
Lol, you haven't been in London I guess... There is some red lights for 10min like..
```

---
## \#32 Posted by: sunnyD Posted at: 2018-07-04T18:13:10.388Z Reads: 407

```
I had assumed my opinion would be faulty at some point. Thats why I tried to cover my ass by saying people should be able to change it :wink:
```

---
## \#33 Posted by: Deckoz Posted at: 2018-07-04T18:33:44.308Z Reads: 404

```
[quote="wafflejock, post:24, topic:60879"]
I’ve accidentally left my board on overnight more than once
[/quote]

I left my evo plugged in for two weeks.. lost 1volt. Rode 37 miles... I don't see a need for auto off either but.... To each their own...
```

---
## \#34 Posted by: Martinsp Posted at: 2018-07-04T18:34:29.642Z Reads: 408

```
I don't think that an opinion can be faulty... Everyone has their own..

Yeah good point, I was thinking since there is a lot of different things that people want I may do it all in "arduino" code. Like upload the bootloader and let people reprogram it easily with something like an arduino uno with arduino IDE or any USB to uart converter. So it would be fairly easily customisable.

There will be some setting that can be changed with hardware like I said, but if someone wants to   make some bigger changes you will be able to.
```

---
## \#35 Posted by: wafflejock Posted at: 2018-07-04T18:43:07.114Z Reads: 407

```
If it's 1hr and let's say 25ma then it's 25mah of power drained with a 5000mAh battery it's negligible savings huge amount of the power consumption is when accelerating or hill climbing.  The area under an amperage curve/graph basically tells you the power consumption higher draw over more time is more power consumed (that times voltage if you really want wattage but can proportionally compare the area under the amperage over time to see power consumed).

Just not worth an accidental cut off for the savings benefit, I can see it for safety of not leaving the board on overnight in case it's already close to discharged or for cutting power to peripheral devices like lights or Bluetooth modules or other displays.
```

---
## \#36 Posted by: Silverline Posted at: 2018-07-04T19:11:22.623Z Reads: 389

```
I would love auto power off.... where i live we dont have massive traffic at all. So given the option to choose, is pretty darn cool of you @Martinsp

Btw. received your "old" antispark yesterday.... nice made :-)
```

---
## \#37 Posted by: TarzanHBK Posted at: 2018-07-05T08:44:58.628Z Reads: 392

```
To summerize it:

* Most of the people would love to get a push-to-turn-on-switch
* We need a programmble auto-turn-off switch, including a hardware switch
```

---
## \#38 Posted by: Andy87 Posted at: 2018-07-05T09:46:44.656Z Reads: 392

```
I fully agree with @TarzanHBK.

@Martinsp what you think will be the max current the switch will be able to handle?
```

---
## \#39 Posted by: Martinsp Posted at: 2018-07-05T10:26:19.906Z Reads: 420

```
The push to start/turn on will be for both versions. Then there will be user choose-able mode with pushbutton to turn off or auto turn off which will be hardware variable from 5minutes to 45minutes 

I will probably go for 100 amps fuse limited since the 100 amps fuses are in most cases not hard to get locally in case the original one blows. Alternatively you could bypass the fuse and go around 150A for a few seconds with 200 peak but that will have to be tested, after the testing I will be able to give you exact numbers. But the above is what I am aiming for.
```

---
## \#40 Posted by: Martinsp Posted at: 2018-07-06T19:19:42.668Z Reads: 438

```
Hello,
so after a quick redesign to implement the features we discussed, here is a 3D render before I have images of the actual switch to show you.
![brd|690x297](upload://AplKZn1NwKhVMX59VLUpQMLDfYQ.png)

There are a couple of components missing and wires of course but this will do for now.

So the way it will work is, there are 3 pads at the bottom to the left of "with BTN" text. The center pad can be shorted with either one of the side ones. As you may guess, the pad on the right, next to the "with BTN" will enable the mode where the switch will turn on with a push and turn off only when pressing a momentary pushbutton that can be connected to the molex connector on the left side of the PCB. There can be an LED/backlit button connected too just like regular switches.
 Shorting the center one with the one on the other side will enable the auto turn off feature. The time after which the switch will turn off can be set with the small trimmer potentiometer to the right of the "with BTN" text.
All of these settings will be user settable so you can try either one and see what you like.

For both versions, there will have to be motor phase wires connected (just thin ones for sensing to make it simpler to solder, will be included) in order for the switch to work, and to be able to turn the system completely OFF. I will do a detailed explanation and how-to once I have the finished product in my hands.
```

---
## \#41 Posted by: Andy87 Posted at: 2018-07-07T08:34:32.546Z Reads: 379

```
I have a question regarding the potentiometer.
Is it possible that the settings can be changed by vibrations of the board?
I mean for example I set to auto off after 20min,
during my ride the poti becomes lose and change to the minimum value.
```

---
## \#42 Posted by: banjaxxed Posted at: 2018-07-07T09:32:35.622Z Reads: 371

```
Hot glue when you have it at the time you want would take care of that

But I doubt it
```

---
## \#43 Posted by: Martinsp Posted at: 2018-07-07T09:32:50.675Z Reads: 372

```
That's a good point, I will try to find one that's the hardest to turn. I think that while it may turn, the weight of it (the spinning part) is too low to overcome the friction. But we will see thank you for reminding me!
```

---
## \#44 Posted by: koralle Posted at: 2018-07-07T10:17:02.782Z Reads: 363

```
Very nice project! For me auto off will be an important feature since I removed all leds from the board (in order not to attract pesky cops). Now the only way to tell if it is switched on is looking at the capacity tester. Someone recently brushed against the on button while board was lying in living room, board was already pretty empty. Rainy days, stayed on for up to a week I guess. Cells at 2.45-2.5v. Fml
```

---
## \#45 Posted by: Martinsp Posted at: 2018-07-07T10:30:37.905Z Reads: 377

```
I think you could save the cells with low current charging, I think this because datasheets for cells measure capacity down to 2.5V. 

Thank you! You could add a small 3mm LED somewhere on your board that is not that easy to spot. There is an output for LED on the Button connector on the PCB.
```

---
## \#46 Posted by: Martinsp Posted at: 2018-07-12T19:24:48.495Z Reads: 390

```
Hello everyone, just a quick update. 
I have received all the parts today and here is the first unit that I am going to iron out all the wrinkles in the firmware as well as add the features we discussed above. It is missing the MCU and needs cleaning but firmware first.
![DSC_0862|690x388](upload://6AZC7rmyJC6CQxPIOuUXj9YV4sG.JPG)

Now as I received a lot of requests of customers to bypass the fuse for them, I am thinking that I will do that as a standard, only a few people wanted the fuse and pretty much everyone has over-current controlled either by the BMS or ESC. On the picture that is 100A fuse "wire"
```

---
## \#47 Posted by: Maxid Posted at: 2018-07-12T19:44:27.769Z Reads: 377

```
That looks as tiny as the one you sent me - how is the size really? And how much will this cost when you start selling them?
```

---
## \#48 Posted by: Martinsp Posted at: 2018-07-12T19:52:14.756Z Reads: 383

```
This one is a little bigger, it is 25.5mm (1") * 40mm (1.57") *9.5mm (0.37")
The price will be higher than the regular switch since this has a  lot more components but at the moment I can not give you an exact number since the BOM is not finalized. But I think it will be around 35-40€ I will have to calculate all the costs to give an exact number, it will be on the product page as soon as I have a stable number and an update here.
```

---
## \#49 Posted by: Martinsp Posted at: 2018-07-22T16:53:26.042Z Reads: 383

```
Hello everyone,

I have the first batch of switches ready but unfortunately it is not for sale yet. Long story short, I dont feel confident with them enough to release them. What happens is that the firmware was tweaked for my dual setup using VESCs 4.12, FOCBOX, FSESC 6.6. I assumed that that the setup would not change much apart from the battery voltage being on the output of the VESC when in OFF state because the gates of the FETs are pulled to ground, I accounted for that but what I was not expecting is that the motor rotation sensing did not work as predicted on 1WD, 2WD and 4WD setups. 

So I am sorry but since I want this to be reliable because some of you want the switch "take control" over your battery almost completely I dont want to release a half working product. The project is still alive and will be worked on by us, what will happen is there will be a new revision of HW and FW soon to improve on the new discovered problems.

If you have any more suggestions I am open to discussing them with you. :slight_smile:
Martin.
```

---
## \#50 Posted by: Vanarian Posted at: 2018-07-22T18:27:51.522Z Reads: 357

```
Nice job there, keep it up!

One question though : does it also act as anti-spark? Do you plan on adding push ON / hold OFF?
```

---
## \#51 Posted by: Martinsp Posted at: 2018-07-22T18:32:41.940Z Reads: 347

```
Thank you! :slight_smile:
 It is just like as if you took a regular anti-spark switch but replaced the regular pushbutton with a microcontroller that senses the rotation of the motor, if it starts rotating it will turn the board on as if you pushed the button. There will be 2 modes, one will be a timer that will turn off after some (adjustable) time and the other mode will only turn the board off if you press and hold the button for 2 seconds. Of course, the modes will be user changeable.
```

---
## \#52 Posted by: Maxid Posted at: 2018-07-22T19:02:34.654Z Reads: 333

```
Just recently realized that @JTAG has this feature now also in his BMS (which is open source) - maybe check how he was doing it and learn from there?
```

---
## \#53 Posted by: Martinsp Posted at: 2018-07-22T19:42:48.109Z Reads: 341

```
Thank you for letting me know, I have been following that project almost from the beginning. I will have to take a different approach however. I will see how it turns out, I am sure I will figure something out or as you say learn from other people maybe I am missing something. Most probably thats the case :D
```

---
## \#54 Posted by: banjaxxed Posted at: 2018-07-22T23:23:06.158Z Reads: 332

```
Good stuff Martin that's very responsible.

GitHub has @JTAGs source and it should be findable

But not sure if licensing slows for a commercial reuse like this
```

---
## \#55 Posted by: Martinsp Posted at: 2018-07-22T23:29:54.056Z Reads: 337

```
The problem is that I think JTAGs BMS uses the UART to communicate with VESC regarding the motor rotation sensing which is not possible if the VESC is OFF completely. I may be wrong, I need to catch up on the improvements of his BMS. It may have been as much as a month since I looked at it closely. 
And yes there might be an issue but I am not sure since I am not using the same hardware as him. If so, there is more than one way to tackle the problem, I think I have solved it about an hour ago but I will leave that to tomorrow. Solving these things at 1am never ends well for me :D
```

---
## \#56 Posted by: banjaxxed Posted at: 2018-07-22T23:32:42.546Z Reads: 324

```
Canbus get a little power from the vesc when the wheel is turned afaik. So although not using the canbus protocol, the bms senses the power passed through and turns on the board, again afaik
```

---
## \#57 Posted by: Martinsp Posted at: 2018-07-22T23:37:34.117Z Reads: 341

```
Oh yeah thats true, as the motor spins the voltage powers the VESC on as discussed in other threads before. Thats a pretty clever solution. I will take a look and experiment tomorrow, if it would need too much hardware and hence increase the physical size of the switch I will have to find a "better" way for this application and keep it small.
```

---
## \#58 Posted by: JTAG Posted at: 2018-07-23T16:11:44.007Z Reads: 387

```
[quote="Martinsp, post:55, topic:60879"]
I think JTAGs BMS uses the UART to communicate with VESC
[/quote]

[quote="Martinsp, post:57, topic:60879"]
if it would need too much hardware and hence increase the physical size of the switch I will have to find a “better” way for this application and keep it small.
[/quote]

Yeah "my" (actually @willumpie82 's ) method is indeed extremely complex!
```

---
## \#59 Posted by: Martinsp Posted at: 2018-07-27T20:00:28.821Z Reads: 401

```
Great news!

I have finished all the necessary changes in hardware and software as well as bench testing and real world testing. The problem turned out to be the precharge circuit, now the switch is tested and working flawlessly with 13S and 11000uF capacitors which is equivalent to 8 FOCBOXes in parralel on 13S! 
Here is a quick (and quite shaky :/ ) video from todays testing. I have been starting and stopping the switch for several hours in both modes and I am happy to say that it works well. :slight_smile:
I removed the audio track because it was so windy that you could not hear a word anyway. 
At the beginning of the video I point to the rear light that is powered from the 5V from the VESCs to demonstrate it is off, same for the remote. This was recorded in the pushbutton mode which requires to be held for 2 seconds to turn off, than it can be started again with pushing the board.
https://youtu.be/s6t7ZrLk0ko 
 
You can expect better looking instructional video soon! The switch will be available at the beginning of next week! I am so excited!:heart_eyes::heart_eyes::heart_eyes:
Thank you all for being so patient and understanding, Martin.
```

---
## \#60 Posted by: Andy87 Posted at: 2018-07-27T20:25:44.285Z Reads: 382

```
A bit off topic, but how you like the alien power remote? Can you recommend it?
```

---
## \#61 Posted by: Martinsp Posted at: 2018-07-28T19:33:02.806Z Reads: 371

```
It is pretty good, I have not had the signal fail in a long time. The downside is that it is not slim, I am planning on 3D printing a better shell for it. I just struggle to find the free time right now :/
```

---
## \#62 Posted by: brenternet Posted at: 2018-07-28T19:47:20.770Z Reads: 377

```
Good progress, not sure how your last post got so little notice. Looking forward to this personally.
```

---
## \#63 Posted by: DAddYE Posted at: 2018-07-29T22:23:58.024Z Reads: 387

```
Looks cool!!! Good job!!!
```

---
## \#64 Posted by: Martinsp Posted at: 2018-08-02T19:40:14.600Z Reads: 396

```
Hello everyone!

I am very excited to finally announce to you that the [**push to start switch is available for order now!**](http://electricskateboard.repair/index.php?id_category=24&controller=category) with a launching sale! Get yourself one [here](http://electricskateboard.repair/index.php?id_category=24&controller=category)
If you want to you can choose to buy one with or without the pushbutton. There was a small change, now you will not need to solder bridge the pads to change modes, I put a sliding switch there to make it easier and quicker. :slight_smile:

Be sure to scroll down and check out the detailed instructions on how to do everything with the switch from start to finish! Hope that the instructions cover all of your questions, if not let me know! :) 

I have been riding with this final version of the switch in the timer mode for the last week and a few days and I have to tell you it is AWESOME! I may be a little bias but I dont have to worry about forgetting the board turned ON since I store it in the garage, I would not notice. Now I just leave it there and it takes care of itself. 

And lastly, I want to thank everyone for the suggestions on improvements, I would not be able to get to this point without you. And also, thank you for your patience. :slight_smile:

Martin.
```

---
## \#65 Posted by: Andy87 Posted at: 2018-08-02T21:06:14.515Z Reads: 362

```
Nice work👍
Just ordered two. Can’t wait to test them out!

One thing you maybe want to add on your website. In the description mentioned that it works as anti spark as well. Good to know for people who not familiar with it.
```

---
## \#66 Posted by: Martinsp Posted at: 2018-08-02T21:24:13.697Z Reads: 357

```
Thank you for the order and also for your recommendation, I will to that. :)
```

---
## \#67 Posted by: linsus Posted at: 2018-08-03T07:59:36.548Z Reads: 355

```
Looks promising, reasonable price as well, will order one when I stop beeing lazy and finnish my stealth build :)
```

---
## \#68 Posted by: Vanarian Posted at: 2018-08-04T18:30:35.508Z Reads: 364

```
http://sarakha63-domotique.fr/wp-content/uploads/2017/03/Shut-up-and-take-my-money.jpg
```

---
## \#69 Posted by: b.sk8 Posted at: 2018-08-07T22:44:38.271Z Reads: 365

```
Hi @Martinsp

Do you think this push to start switch  can be used with dual fesc 6.6 aluminum case? I want to by pass on and off switch![IMG_20180725_192832|375x500](upload://ylmPcZApYRG0yxE1KY00Rz0bZQx.jpg)
```

---
## \#70 Posted by: b264 Posted at: 2018-08-07T23:22:08.182Z Reads: 347

```
What is the auto-poweroff time set at?  At least an hour?
```

---
## \#71 Posted by: Martinsp Posted at: 2018-08-07T23:30:29.605Z Reads: 355

```
@b.sk8 Yes it can be used with it, you will just either have to leave the pushbuttons on the ESCs in ON position or just bypass them internally. Either way works.

@b264 The auto off is user adjustable from 5 to 45 minutes. I wanted to go higher a little on the upper limit but since the potentiometer has only 200° I think it was so increasing the range would make it harder to choose the desired time with some reasonable precision
```

---
## \#72 Posted by: b.sk8 Posted at: 2018-08-08T13:42:46.127Z Reads: 345

```
@Martinsp I take your word for it and ordered one. This is a push button so, I am not sure how to leave it at ON. Is one switch enough to operate dual Fesc?
```

---
## \#73 Posted by: Martinsp Posted at: 2018-08-08T15:19:15.921Z Reads: 341

```
The push button on the fsesc is latching which means that it stays in position after you press it like a light switch would but on the push to start switch the pushbutton is momentary so it returns to default position after being pressed like a door bell switch for example

Yes one is enough you can split the output between them
```

---
## \#74 Posted by: Jasonkimberson Posted at: 2018-08-08T16:25:24.547Z Reads: 334

```
Ordered two of these and two of the older ones, can’t wait to try it out
```

---
## \#75 Posted by: Komamtb Posted at: 2018-08-14T09:13:25.873Z Reads: 347

```
![IMG_20180814_120159|374x500](upload://ye6YyI0isBOdtWzU76KjUqxbhvT.jpg)![IMG_20180814_120128|374x500](upload://5Ii7AOHzQwa6pmlxAQDY7TQnlYK.jpg)
```

---
## \#76 Posted by: Martinsp Posted at: 2018-08-15T19:54:38.900Z Reads: 323

```
@Komamtb That looks very clean, I like it!

BTW, I have the same Fiio X1. Do you also find it as if the sliding wheel sometimes missed a step? Maybe I just have it worn out or something
```

---
## \#77 Posted by: Komamtb Posted at: 2018-08-16T09:28:54.048Z Reads: 320

```
Yes it does, but the new FW helped a bit. Fiio do know the issue with some of the x1 devices.
```

---
## \#78 Posted by: Martinsp Posted at: 2018-08-16T21:31:01.976Z Reads: 318

```
Aha, thank you I had no idea there was a new FW... I may get around to asking them one of these days, I learned to live with it probably though :D
```

---
## \#79 Posted by: Martinsp Posted at: 2018-08-18T17:02:45.412Z Reads: 308

```
Just a heads up, the switches are available for backorder! :slight_smile:
They will ship out on Wednesday, just a few days to go! Get yours [**here**](http://electricskateboard.repair/index.php?id_category=24&controller=category) 
You can choose one with or without the pushbutton. Modes are user changeable, I have been asked if it is possible a lot, so yes it is!  :) 

Martin.
```

---
## \#80 Posted by: uigiroux Posted at: 2018-09-02T00:12:25.216Z Reads: 294

```
I'm really considering getting one of these, but I also will be using a DieBieBMS, which I think has this 'push to start' feature also, though I think it requires modifying the PCB or some of the boards components. So would this be easier to use if I wanted that feature?  I don't care about the cost, just want the feature with the most reliability and easiest to implement. Thoughts? :smile:
```

---
## \#81 Posted by: Jc06505n Posted at: 2018-09-02T00:15:49.261Z Reads: 292

```
As of right now at least 3 stand alone products have the potential to execute the list to start feature ( This antispark, your BMS , and the Unity. It seems this, for now, is the easiest as it requires you to just solder the connection to a phase wire. The only hang up would be for if/when the antispark dies
```

---
## \#82 Posted by: uigiroux Posted at: 2018-09-02T00:26:12.006Z Reads: 291

```
Lol, well I ended up just buying it anyway haha.  If I put a loop key right before this, going from the battery, like it shows in the schematics, would that solve that issue?
```

---
## \#83 Posted by: Jc06505n Posted at: 2018-09-02T00:38:24.445Z Reads: 290

```
It would be a redundancy, I don’t know enough about the topic to say if having an anti spark key levitates the potential for an antispark to pop
```

---
## \#84 Posted by: SeanHacker Posted at: 2018-09-02T00:40:09.451Z Reads: 289

```
You don't need a loop key if you have this. That's what this alleviates. ;)

Just as @Jc06505n said. Redundant.
```

---
## \#85 Posted by: Martinsp Posted at: 2018-09-02T11:35:08.494Z Reads: 314

```
Hi,

I am not sure if you need to modify the PCB of @JTAG DieBieBMS, you would need the newest firmware I would assume if you bought it before it had this feature. Not sure 100% though...

Pretty much any ESC with integrated switch has the pottential to have this feature implemented as long as the MCU on the ESC is connected/has the ability to control the switch.

I do recommend having a loop key somewhere on your board in every case, maybe hidden somewhere so that you can leave it in without it being eye catching in a bad way and just have it there for safety. 
I have tested this switch with high capacitive loads and I strongly believe it is not going to fail like some of the simpler switches that just use the precharge RC circuit as in the original vedder/fechter schematic. Most cases of switches failing is not while they are fully on but when they are changing states especially from OFF to ON because of the inrush current that is going through the switch while the capacitors are charging. The microcontroller has much more predictable operation.
I have not announced this yet but since the last batch of the regular switches they were also been using microcontrollers to make sure they are as reliable as they can be. :slight_smile:

Martin
```

---
## \#86 Posted by: kalebludlow Posted at: 2018-09-05T04:40:56.912Z Reads: 276

```
DIYeboard ESC also has the same feature
```

---
## \#87 Posted by: Hanok Posted at: 2018-09-05T16:39:21.990Z Reads: 295

```
Hi.
I got the switch.
But it doesn't work.
This part produces a lot of heat.
![KakaoTalk_Photo_2018-09-06-01-29-40|500x500](upload://9GguVJNgxeOw9S3gyuFjfpAyvI8.jpeg)
Can you help me?
```

---
## \#88 Posted by: Martinsp Posted at: 2018-09-05T17:00:34.025Z Reads: 289

```
Hi @Hanok, 

Can you please PM me what the switch is doing or if it works? As well as a picture of the PCB so I can see better.

Some pushbuttons are configured internally to power the LED from just the two wires as you have it connected, the part you are pointing to is a voltage regulator for the MCU and it is not designed for it. 

Dont worry, I will sort this out for you.

Martin.
```

---
## \#89 Posted by: craigthemachine Posted at: 2018-09-05T17:07:17.949Z Reads: 297

```
My switch works, however I did notice having trouble turning it off “manually” a bit of a challange. “Hit and miss” 

Must be sensitivity to the phase wires or faint signals from the ppm remote that are sent to the Focbox 

 I over came this by installing another switch To cut the connection phase wires to the anti spark. 

Other than that, it seems to be working ok.
```

---
## \#90 Posted by: Hanok Posted at: 2018-09-05T17:09:20.608Z Reads: 295

```
LED connected.
The battery is connected and does not operate at all when the switch is pressed.
The momentary switch is being used.

![KakaoTalk_Photo_2018-09-06-02-05-12|500x500](upload://oVF1AVTy41xstvZpJpOMzsO4Dy7.jpeg)
```

---
## \#91 Posted by: Martinsp Posted at: 2018-09-05T17:20:24.440Z Reads: 288

```
Aha I see, 

I will replace the unit for free for you. I test all of them before they are packaged but maybe something happened during shipping or whatever. I found your order so I have your address. I will PM you the details.
```

---
## \#92 Posted by: Hanok Posted at: 2018-09-05T17:23:42.443Z Reads: 280

```
Thanks.:울프:
```

---
## \#93 Posted by: craigthemachine Posted at: 2018-09-05T17:41:19.328Z Reads: 279

```
It appears the switch on option is “only” via the phase wires. Because I can’t power by switch either. I can only turn the anti-spark on by spinning the motor.
```

---
## \#94 Posted by: craigthemachine Posted at: 2018-09-05T17:42:44.383Z Reads: 278

```
Is that how the switch intends to work?

1. Only on via phase wires 
2. Auto-off (time based)
3. Manual off (switch)
```

---
## \#95 Posted by: Martinsp Posted at: 2018-09-05T17:44:44.134Z Reads: 270

```
Yes the switch turns on when you push on your board which spins the motor and turns the system ON.
```

---
## \#96 Posted by: craigthemachine Posted at: 2018-09-05T17:46:35.439Z Reads: 278

```
Thought so... because I had a wtf moment when trying to “only” use the push switch. It wouldn’t power. Until I installed the phase wires. 

Maybe you should include that as a revised version. 🤷🏽‍♂️
```

---
## \#97 Posted by: Martinsp Posted at: 2018-09-05T17:49:12.230Z Reads: 276

```
Thank you for the recommendation, it is one of the improvements on the list for the next batch :D
```

---
## \#98 Posted by: craigthemachine Posted at: 2018-09-05T17:50:30.034Z Reads: 281

```
Perfect ! I would like to have one as soon as . 😃
```

---
## \#99 Posted by: Komamtb Posted at: 2018-09-07T15:44:25.702Z Reads: 280

```
Anyones else switch never turns off..?
```

---
## \#100 Posted by: Martinsp Posted at: 2018-09-07T19:12:02.788Z Reads: 288

```
Hi @Komamtb,

Can you please PM me pictures of the switch and connections? What you are describing sounds like there is not a good connection somewhere which triggers the MCU.

Martin.
```

---
## \#101 Posted by: CarbonV Posted at: 2018-09-10T09:55:19.697Z Reads: 291

```
Just received my switch from @Martinsp! 
Was well packaged and looks great. Will test very soon. 
![IMG_20180910_115248|666x500](upload://lTIbH4jv4k5B0kZ99ARLAzEP3OJ.jpg)
```

---
## \#102 Posted by: sofu Posted at: 2018-09-25T22:03:44.273Z Reads: 286

```
Isn't this a pretty common issue with switches? Where the switch will fail closed and you can't turn it off? I've had it happen with all my switches: Vedder, Lunacycle, even the dinosaur series from antispark haven... I've yet to find one that won't fail closed on me. Hopefully the FATboy mini sparky won't...
```

---
## \#103 Posted by: b264 Posted at: 2018-09-25T22:06:58.674Z Reads: 279

```
think we should focus on them not failing at all LoLz
```

---
## \#104 Posted by: Eboostin Posted at: 2018-09-25T23:33:04.659Z Reads: 286

```
Wouldn’t it be better to have them fail on? Would suck if it failed off and threw someone off their board
```

---
## \#105 Posted by: barajabali Posted at: 2018-09-26T01:19:11.985Z Reads: 282

```
Hows the testing going on this ? Early backers?
```

---
## \#106 Posted by: garseng Posted at: 2018-09-26T02:13:07.085Z Reads: 283

```
I’ve been using this switch for over a month..so far so good.
```

---
## \#107 Posted by: Jasonkimberson Posted at: 2018-09-26T02:46:34.307Z Reads: 288

```
I bought the switch and realized you can either only have it on a timer to shut off or you can have it push button for 3 seconds off.  You can’t have both.  Also, with the push to start switch, you have to push to start, you can’t push the button to start...


![image|350x263](upload://zLiGZTNi0cQWHh1aS1hlVud7Sfx.gif)
```

---
## \#108 Posted by: barajabali Posted at: 2018-09-26T03:56:09.365Z Reads: 281

```
Thanks for the feedback.i may pick one up for a small project
```

---
## \#109 Posted by: sofu Posted at: 2018-09-26T18:12:59.947Z Reads: 279

```
Fail closed means they get stuck on so you can't turn them off
```

---
## \#110 Posted by: Martinsp Posted at: 2018-09-28T16:29:26.210Z Reads: 293

```
Hello everyone,

sorry for not replying here or in PMs. I was unfortunately busy moving the shop to a different/new location. We should be back on track with orders and other stuff already. I have replied to everyone I think in PMs and emails but if you have not received a reply please just let me know I may have unintentionally skip someone.

Now to reply to you here: 
@sofu  yes 90% of mosfet switches fail this way. I have destroyed intentionally around 25-30 to find out how and why it happens when designing my own. So there are some that fail due to overload but that was only possible to achieve with static loads exceeding 100A for loner periods of time which burned the mosfets or heared them up to a point where they would malfunction and eventually break. The majority of failed FETs however is when they are turning on. This is due to high current spikes that are created due to the capacitors on VESCS. For this I have made a bank of capacitros (11000uF so equivalent to for example 8 FOCBOXes in parallel) and tried to switch that on and off repeatedly (discharging the caps in between cycles of course) to make sure that the switches are capable of this. I was not able to do this successfully with regular switches thats why all the new ones (push to start and the "regular" antisparks) use and MCU to control the gate of mosfets more precisely. Now that is not to say that my switches dont fail, they do. The failure rate of push to start switches has been 2% so far. IMO that is pretty good so far.

@barajabali I think I have the earliest unit out there. I use it on my daily without issues. It is not under too much stress however. I have dual 10S 245kv on FOC with regular 4.12 VESCs running at 80A motor max, 60A battery. The maximum real current I am able to pull going up hills etc is 55A. I dont live in a particularly hilly area but not a lot of boards exceed similar current anyway. 

@Jasonkimberson I am aware of this and new batch is currently under testing. This one will include turn on possibility with button as well. But thank you for letting me know anyway :) I may do some kind of a swap for the people that need/want the feature but have one of the earlier units.

Martin.
```

---
## \#111 Posted by: sofu Posted at: 2018-09-28T20:51:36.811Z Reads: 273

```
Thanks for the explanation! I fully expect this new warranty replacement lunacycle switch i have to fail closed within the month, so I'd be more than happy to "real world test" one of your switches :stuck_out_tongue:

Just kidding but also kinda not really kidding... I'm getting super fed up with these luna switches 🙃
```

---
## \#112 Posted by: nuttyjeff Posted at: 2018-09-29T07:56:53.920Z Reads: 264

```
Anyone have any idea which side the input and output of this switch are at? And also, which side the slide button should be for the push to start mode?
```

---
## \#113 Posted by: Martinsp Posted at: 2018-09-29T08:01:50.329Z Reads: 262

```
@nuttyjeff You may have missed the instructions at the bottom of this page http://electricskateboard.repair/index.php?id_product=44&controller=product
```

---
## \#114 Posted by: nuttyjeff Posted at: 2018-09-29T08:02:37.072Z Reads: 260

```
Damn missed it! thanks!
```

---
## \#115 Posted by: bigben Posted at: 2018-09-29T19:59:39.280Z Reads: 261

```
I've just installed this and so far is working faultlessly.
What a cool idea. I've already done away with a voltage meter and use an app. Now done away with the switch. Now just have to  do away with the charge port and were good to go. Thanks @Surfer for putting me on to this! (or was it @sayekim?)
```

---
## \#116 Posted by: DavidBanner Posted at: 2018-09-29T20:04:00.091Z Reads: 262

```
[quote="bigben, post:115, topic:60879"]
I’ve already done away with a voltage meter and use an app
[/quote]

I've done the same. Do you ever miss having the LCD display?
```

---
## \#117 Posted by: bigben Posted at: 2018-09-29T20:06:36.620Z Reads: 263

```
No, I just look at the app which I trust more than my 50 cent display!
```

---
## \#118 Posted by: b264 Posted at: 2018-09-29T20:21:38.320Z Reads: 273

```
[quote="bigben, post:115, topic:60879"]
I’ve already done away with a voltage meter
[/quote]

Me too.  The charge port is just fine for that...

![20180414_152813|690x345](upload://2yXnEejZnCtRR68kpwalNBZx0s4.jpeg)
```

---
## \#119 Posted by: bigben Posted at: 2018-09-29T20:23:30.820Z Reads: 265

```
Not so daft.
```

---
## \#120 Posted by: b264 Posted at: 2018-09-29T20:24:52.199Z Reads: 266

```
@bigben that thing is the most useful thing I ever made, and it plugs into every board, including the commercial boards...just ride with it in your pocket.  It's in my pocket right now

Besides that, you get a feel for how far your boards go and almost never need to check unless you're pushing it further than usual.  But just having it in your pocket gives you the good feeling that you could know at any second.  Despite not actually checking.
```

---
## \#121 Posted by: Martinsp Posted at: 2018-09-29T20:26:58.315Z Reads: 255

```
Thank you @bigben for the feedback!
```

---
## \#122 Posted by: sayekim Posted at: 2018-09-29T20:27:20.593Z Reads: 255

```
Oh now I get it. Yeah I already have one in my pocket. It’s my phone with the app.
```

---
## \#123 Posted by: bigben Posted at: 2018-09-29T20:34:09.078Z Reads: 264

```
Possibly a bit like me, for most people this is under their radar or don't really understand quite what this little switch will do for them. It doesn't turn on with the slightest movement so the board doesn't turn on with some manhandling, only a good spin of the wheel and it fires into action.
For now I'm converted.
```

---
## \#124 Posted by: moon Posted at: 2018-09-29T20:37:13.598Z Reads: 255

```
Tremendous
```

---
## \#125 Posted by: Martinsp Posted at: 2018-09-29T20:37:27.583Z Reads: 258

```
There is a threshold for it exactly for that reason. I had it in the first testing stages and it turned on when sometimes i dragged the board when carrying it by the front truck up stairs for example so yeah, it needs to be a relatively easy push to get the motors going.
```

---
## \#126 Posted by: Jasonkimberson Posted at: 2018-10-02T19:14:12.448Z Reads: 263

```
Hi martin,  dm’ed you!
```

---
## \#127 Posted by: janpirate Posted at: 2018-10-10T13:41:16.352Z Reads: 261

```
hello martin,

please check you PM.
```

---
## \#128 Posted by: Bibzz Posted at: 2018-11-17T17:44:26.215Z Reads: 257

```
Same Martin,

Check you PM
```

---
## \#129 Posted by: Martinsp Posted at: 2018-11-22T18:58:49.762Z Reads: 253

```
[![image|690x400](upload://nNcnBTWExZtFSZB1StqfhnAxbWn.jpeg) ](http://electricskateboard.repair/index.php?id_category=14&controller=category)


Click the picture or [this link](http://electricskateboard.repair/index.php?id_category=14&controller=category) to go to the website. :slight_smile:
This is the last batch before a small break due to new products coming in and they need some finishing touches before they will be up for sale.  
BR, Martin.
```

---
## \#130 Posted by: banjaxxed Posted at: 2018-11-22T21:11:01.189Z Reads: 240

```
Nice one Martin, I had to order one, probably this has been gone through before but can you use a multimeter to determine the time it will shut off?
```

---
## \#131 Posted by: Surfer Posted at: 2018-11-22T21:23:15.838Z Reads: 239

```
It is even easier, it has a potentiometer to select from 5 mins to 45 mins.
```

---
## \#132 Posted by: banjaxxed Posted at: 2018-11-22T21:27:42.107Z Reads: 253

```
Yeah but a potentiometer how to tell if you’ve turned it up to 11

https://youtu.be/s9F5fhJQo34
```

---
## \#133 Posted by: Martinsp Posted at: 2018-11-22T21:28:59.871Z Reads: 249

```
Actually noone asked so far. At the bottom of the product page there is a pdf with instructions, you can find a picture with angle corresponding to time. I was thinking about having it like setting current on diy printers but I don't suggest having it powered and poking screwdriver in honestly, to avoid damage.
```

---
## \#134 Posted by: Surfer Posted at: 2018-11-22T21:30:21.590Z Reads: 253

```
![Screenshot_20181122-222914__01|690x260](upload://bURtTgrZAZi3OV5WHdG9eJa7CAt.jpeg)
```

---
## \#135 Posted by: Surfer Posted at: 2018-11-22T21:38:32.388Z Reads: 249

```
Did already start black Friday in your web?
I'm impatient :)
```

---
## \#136 Posted by: Martinsp Posted at: 2018-11-22T21:43:33.003Z Reads: 252

```
Thank you for sharing the pic!

Yes, it will be longer than 24 hours since different timezones etc... :)
```

---
## \#137 Posted by: Martinsp Posted at: 2018-11-25T15:09:22.643Z Reads: 243

```
There are a few units left for sale! The sale will only continue for the next 32 hours, dont miss out!
[CLICK HERE](http://electricskateboard.repair/index.php?id_category=14&controller=category)
```

---
## \#138 Posted by: DAddYE Posted at: 2018-11-25T16:45:44.205Z Reads: 237

```
I got a switch (normal one) a while back from @Martinsp and I can tell it’s the only one that didn’t break so far. Pretty pleased
```

---
## \#139 Posted by: CarbonV Posted at: 2018-11-25T18:50:10.767Z Reads: 231

```
My switch never worked, wrote him on here, send an email to the support mail on his site and never got anything back.

Edit: I'm getting an new switch send, thank you foe the support Martin.
```

---
## \#140 Posted by: Martinsp Posted at: 2018-11-25T18:54:10.955Z Reads: 224

```
Hi,
sorry to hear this, I must have missed it. give me a moment.
```

---
## \#141 Posted by: Indiangummy Posted at: 2018-11-25T18:54:35.022Z Reads: 240

```
Hey I got an error after I completed the checkout and PayPal redirected me to your site. But my payment did go though? Could you confirm the order? Thank you
```

---
## \#142 Posted by: Martinsp Posted at: 2018-11-25T18:56:28.765Z Reads: 245

```
It did, I think it is an error on PP side because during this sale it is the first time it happened so maybe they are experiencing an overload on servers or something. I will have to wait for the sale to be over to figure it out. Anyway, your order has gone through OK. Thank you.
```

---
## \#143 Posted by: BigBrit Posted at: 2018-12-09T11:23:22.343Z Reads: 250

```
@Martinsp any ideas when you might get the switches back in stock?

My mate wants a push to start and I would like one of your switched antisparks
```

---
## \#144 Posted by: Martinsp Posted at: 2018-12-09T11:43:47.620Z Reads: 265

```
Hello,

I am hoping for a new batch before Christmas, however I can not promise that. The delivery times are so delayed that I can not tell you if its next week or two weeks from now, sorry.

And to everyone who ordered switch from around black Friday and later, please excuse the delays, I think due to the black Friday and Christmas the delivery times are delayed. Please dont worry, should your package get lost due to the postal mess or something like that, I can send you a new one or offer you a full refund.

Sorry again for the inconvenience everyone, it is beyond my control unfortunately.
Martin
```

---
## \#145 Posted by: Mich21050 Posted at: 2018-12-09T21:27:17.684Z Reads: 240

```
Any plans on making it open source?
```

---
## \#146 Posted by: 702vegas Posted at: 2018-12-10T00:01:58.729Z Reads: 238

```
Hey Martin. I emailed and dmed you . but no reply
```

---
## \#147 Posted by: StefanMe Posted at: 2018-12-10T06:02:48.494Z Reads: 226

```
Same for  me... i guess he is overloaded with the project at the moment
```

---
## \#148 Posted by: rojitor Posted at: 2018-12-10T09:54:43.435Z Reads: 222

```
Same here. No reply from @Martinsp
```

---
## \#149 Posted by: sayekim Posted at: 2018-12-10T10:01:15.916Z Reads: 224

```
I suppose the guy is on holiday with all our monies and since he’s out of stock and won’t get parts for perhaps another two weeks I think he mentioned, he’s just chilling. 

I don’t blame him. I’d do it too. Don’t worry he’ll be back when he’s back with stock.
```

---
## \#150 Posted by: StefanMe Posted at: 2018-12-10T10:37:21.150Z Reads: 227

```
The problem is, I really need an push to start switch... u don’t wanna drill a hole in my deck and my old one is broken. The order was on two weeks ago and it should take longer than a week to Germany. 

I also don’t wanna blame him, but I wanna know i get this part within the next days or I have to wait for a few weeks...
```

---
## \#151 Posted by: pjotr47 Posted at: 2018-12-10T12:13:02.380Z Reads: 223

```
In our hobby you must have a lot of patience. Many people do projects in their free time...
```

---
## \#152 Posted by: StefanMe Posted at: 2018-12-10T12:59:30.914Z Reads: 224

```
U are wrong. He has a professional shop. This is not a hobby for him. It is a business.

But as I mentioned before. I don’t want to blame him.
I just want to have a delivery range where I can expect the switch.
```

---
## \#153 Posted by: sayekim Posted at: 2018-12-10T13:42:41.170Z Reads: 228

```
If you indeed already ordered while they were in stock then I certainly understand he should take care of those customers. 

Unfortunately there is very little you can do here besides buying another somewhere else that is in stock but I don’t think anyone else has one that is similar with similar price. 

It sucks. You just gotta wait. I am waiting on an order too from someone else for some answers.
```

---
## \#154 Posted by: Martinsp Posted at: 2018-12-10T14:24:37.407Z Reads: 230

```
Id love to be on a holiday TBH. I have school apart from this and it is the exam time again.

I will check whats up with your order and PM you @StefanMe
And also get back to you guys with replies.
```

---
## \#155 Posted by: pjotr47 Posted at: 2018-12-10T14:26:55.829Z Reads: 231

```
So if you have a webshop it it can not be a hobby? :joy:

Many persons here have a normal life with work/school and sell stuff as hobby :

Be happy that we have such a people like @Martinsp, who is developing such a small antispark and is sharing his knowledge. 

A few years ago we had far fewer options and all costs a lot more money.
...Mic drop...
```

---
## \#156 Posted by: s5300 Posted at: 2018-12-10T19:51:41.841Z Reads: 226

```
This is *generally* finals week for college students. Give him a bit of time.
```

---
## \#157 Posted by: JibeBigo Posted at: 2018-12-14T14:17:53.712Z Reads: 217

```
I paid 55$ for a Flipsky one, if you're already overloaded with orders, raise the price.
I can't believe I said this, please save me 2 for my future builds at 35$ xD
```

---
## \#158 Posted by: banjaxxed Posted at: 2018-12-18T14:57:03.450Z Reads: 216

```
I’m loving this too as I’m running out of space with a HAYA build. This will allow me to consider a 13s setup with the advantage of no on/off button to route.

I can wait for stock to return
```

---
## \#159 Posted by: Bobby Posted at: 2018-12-19T06:50:12.377Z Reads: 224

```
Did you make this? How can I get my mitts on one of those pocket battery voltage reader thingys
```

---
## \#160 Posted by: b264 Posted at: 2018-12-19T06:53:50.501Z Reads: 239

```
Yes; I've made a number of them.  I like them better than a gauge in the enclosure because it's one less place for water to get inside, one less hole in the enclosure, one less thing to cram inside, and it's one less thing that can fail.

![20181213_135632|690x388](upload://622R6NNfAVCUbDcC0c6cNxS9OE.jpeg) 

![20181118_205557|690x345](upload://e69iJRqJ1Wh5wVhq0qRdq6urfYt.jpeg) 

![20181118_205522|690x345](upload://2ALCWQbs3EAurHFeENQBbfwilmA.jpeg)

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-use-pm/2992/8573?u=b264
```

---
## \#161 Posted by: Bobby Posted at: 2018-12-19T06:59:31.563Z Reads: 221

```
Are they difficult to make @b264 ? Do you have any tutorials made on this? Id prefer this rather than cutting throught the enclosure for an display
```

---
## \#162 Posted by: pat.speed Posted at: 2018-12-19T10:33:27.395Z Reads: 214

```
Super easy man, You legit just solder the connector pins to where the monitors wires come from
```

---
## \#163 Posted by: b264 Posted at: 2018-12-19T10:37:58.780Z Reads: 218

```
Battery Gauge, JB Weld, 5.5 x 2.1mm barrel connector

Seriously, cheap  <$20

I always have one in my pocket
```

---
## \#164 Posted by: pat.speed Posted at: 2018-12-19T10:39:58.014Z Reads: 217

```
Hot glue works well too and it's easier to get off if you make a shoddy solder
```

---
## \#165 Posted by: b264 Posted at: 2018-12-19T10:41:15.184Z Reads: 221

```
It's not soldered, it's the connector that comes with the battery gauge

edit: oh yeah, it's soldered to the barrel plug

I would not use hot glue though.  If you mix JB Weld correctly and thoroughly and don't touch it for 30 hours, it becomes permanent and won't come apart.
```

---
## \#166 Posted by: Friskies Posted at: 2018-12-19T13:18:30.062Z Reads: 223

```
Honestly why not just get a Bluetooth module for that price.l? Not like it really affects anything else and you don't need to bend over every moment that you want to check the battery voltage. 
Even better get a metr module and you can monitor the battery across your entire ride and even have triggers to send you notifications if you battery is hitting critical levels.
```

---
## \#167 Posted by: Bobby Posted at: 2018-12-19T16:56:43.851Z Reads: 209

```
Because I constantly frankenstein and make new boards a lot. This is universal no matter what board im riding at the time, i can use it. Not to mention my phone battery is a Piece o shit...
```

---
## \#168 Posted by: Bobby Posted at: 2018-12-19T17:06:05.703Z Reads: 208

```
Im sorry but im pretty dumb with the electrical jargon... connector pins where monitor wires huh?? I only taught myself to build and solder this April so im still pretty green. Do i solder certain wires to the dc barrel? Is it just positive and negative? Do i need a certain battery gauge? Is the glue just to keep everything from moving around?
```

---
## \#169 Posted by: pat.speed Posted at: 2018-12-19T21:05:27.024Z Reads: 204

```
Yeah it’s just the positive and negative wire that you connect. You can use any battery gauge you like. The one @b264 is a good one as it shows both percent and voltage, however I have one just for voltage. And yes the glue is just to hold it all together
```

---
## \#170 Posted by: b264 Posted at: 2018-12-19T21:12:45.366Z Reads: 201

```
It's not glue, it's epoxy.  There is a massive difference.  Glue falls apart eventually.  Epoxy is forever.
```

---
## \#171 Posted by: pat.speed Posted at: 2018-12-19T21:14:46.139Z Reads: 202

```
What if you need it apart?
```

---
## \#172 Posted by: b264 Posted at: 2018-12-19T21:21:50.328Z Reads: 214

```
It's only a few dollars worth of parts.

![download%20(1)|230x230](upload://ciFdBxIRFrCPTIn1CrQr8zeXVT9.jpeg)

Never comes apart.
```

---
## \#173 Posted by: Surfer Posted at: 2018-12-19T21:39:11.034Z Reads: 220

```
For similar amount of money and similar work I prefer this one, it gives you the same info plus makes your brick charger a lot smarter, for example how many amps going through, volts, time and watts. Really cheap and useful.
![IMG_20181219_223159__01|640x500](upload://qUtEXo5PKaWJjXlF3LWzQZJ86q9.jpeg) 

7 in 1 OLED Electrical Parameter Meter Power Meter Voltage Current Time Power Energy Capacity Temp Tester Free Shipping 12002965
 https://s.click.aliexpress.com/e/b3K0MHqC
```

---
## \#174 Posted by: b264 Posted at: 2018-12-19T21:44:28.136Z Reads: 209

```
Wow, that's awesome :smiley: Thanks @Surfer 

There are only 999,952 in-stock though, better get them before they run out :smile:
```

---
## \#176 Posted by: Surfer Posted at: 2018-12-19T21:54:49.705Z Reads: 213

```
I use the 20A and I know I never going to charge that fast, o maybe yesus!!
```

---
## \#177 Posted by: StefanMe Posted at: 2018-12-25T12:07:03.774Z Reads: 207

```
I can't get this switch working... in BUTTON mode it works sometimes. At least du have to wait for 10 seconds to switch the boar off (no big deal) but in auto off mode, it never goes off and I can't switch it off manual by the button press. I use it on my FSESC6.6.

Has someone the same problems?
```

---
## \#178 Posted by: sayekim Posted at: 2018-12-25T12:49:17.382Z Reads: 205

```
I don’t think the esc would matter but I use this with dual escapes and no button.

I have set it to switch off at the smallest time  interval of 5 minutes and it works great every time. 
🕓
```

---
## \#179 Posted by: StefanMe Posted at: 2018-12-25T14:59:21.854Z Reads: 203

```
Ok, so it’s slider to the right and potentiometer fill clockwise...? 

I ll try it again later.
```

---
## \#180 Posted by: sayekim Posted at: 2018-12-25T15:17:39.175Z Reads: 203

```
Instructions. 

http://electricskateboard.repair/index.php?controller=attachment&id_attachment=2
```

---
## \#181 Posted by: StefanMe Posted at: 2018-12-25T17:08:25.459Z Reads: 205

```
Yes I know the instructions. Thanks for telling me nothing. :face_with_monocle:

**I can confirm. It does not work with the FSESC6.6. At least not for me. Focbox is working fine... Has anyone else an FESC6.6 with the switch?**
```

---
## \#182 Posted by: pjotr47 Posted at: 2018-12-25T17:22:04.815Z Reads: 208

```
[quote="StefanMe, post:181, topic:60879"]
Thanks for telling me nothing. :face_with_monocle:
[/quote]

The only thing that @sayekim want is help you...
```

---
## \#183 Posted by: StefanMe Posted at: 2018-12-25T17:27:08.012Z Reads: 202

```
U find smart words for EVERYTHING...
```

---
## \#184 Posted by: sayekim Posted at: 2018-12-25T17:48:25.846Z Reads: 209

```
Hold your tits there buddy. 

You want me to read the instructions for you?

Because that is what I would need to do to answer your questions.
```

---
## \#185 Posted by: StefanMe Posted at: 2018-12-25T17:55:41.413Z Reads: 215

```
Sorry i was stressed. Thanks. 

The settings I did was correct. Now it works... not shure why. I removed the shrink... I ll give it some more tries and see how stable it is now.
```

---
## \#186 Posted by: Martinsp Posted at: 2019-02-08T11:56:38.102Z Reads: 222

```
Hello everyone,

so finally after over a month of no stock, its here. I have switches ([Regular switches as well](https://www.electric-skateboard.builders/t/anti-spark-switch-direct-fets-heatsink-metal-led-switch-is-included-100a/50912/134)) in stock.

[Here they are!](http://sprusi.com/index.php?id_product=32&id_product_attribute=0&rewrite=push-to-start-antispark-switch-v7-with-push-button&controller=product)

There is a lot of changes done in this version (V7)! First of all and probably the most usefull of them is that the threshold at which the switch turns on is now adjustable by the end user. This is important because the old switch worked for most builds but if you were using some other ESC than VESC it was a bit of a hit or miss as well if you were using too high or too low kv the threshold was too sensitive which resulted int the switch turning on when it should no etc. Plus now the switch works for e-bikes, e-scooters etc as well if that is your thing :slight_smile:

Second change is that the timer potentiometer is now larger and easier to adjust without shorting things out, an oversight/issue on the first versions because of the lack of space. Also the sliding switch for mode selections is now more robust as well.

Finally, the push button can now turn on and off the switch at any mode not only at "pushbutton mode" which is now called "timer disabled mode" for a lack of a better name :D 

I could go on and on but these were the most important news. Oh and we now have the nicer pushbuttons with power logo in stock!

We have also moved to a new site because we have had too many things to change on the old website so it made sense to make a new one since I wanted to change the name anyway. Of course all of our “old” products and services are still available as before and there is plenty more to come. The new website is [www.SPRUSI.com](http://www.sprusi.com/) and it should be all set up ready to go. Please if you encounter any issues let me know so I can resolve them. :slight_smile:

![4|500x500](upload://cOraDpIa4Hix0r1ubBj61mjDJG0.jpeg)
```

---
## \#187 Posted by: martijntje42 Posted at: 2019-02-08T12:04:39.226Z Reads: 210

```
I can't seem to reach the website. (timed out connection) Are we crashing your servers with too much traffic already?
```

---
## \#188 Posted by: Andy87 Posted at: 2019-02-08T12:12:22.487Z Reads: 205

```
For me it’s working.
I like the test item 😅 need to order one !
```

---
## \#189 Posted by: Martinsp Posted at: 2019-02-08T12:12:51.589Z Reads: 218

```
I have checked and it works for me, even with VPN :/

@ Oh sh** I forgot to delete that! :D thanks
```

---
## \#190 Posted by: martijntje42 Posted at: 2019-02-08T12:15:00.992Z Reads: 215

```
And it works again... no idea
```

---
## \#191 Posted by: CarbonV Posted at: 2019-02-08T13:49:32.526Z Reads: 209

```
Hey dude would you mind replying to my pm now then? :)
```

---
## \#192 Posted by: Martinsp Posted at: 2019-02-08T13:58:18.789Z Reads: 202

```
Thought I was all caught up with replies, sorry. Im on it
```

---
## \#193 Posted by: SeanHacker Posted at: 2019-02-12T23:17:27.539Z Reads: 197

```
Looks like my order shipped. I noticed it says "**Carrier**  International post (tracked)" but doesn't give a tracking number. How are we supposed to track it @Martinsp? Thanks again.
```

---
## \#194 Posted by: Martinsp Posted at: 2019-02-13T13:54:36.598Z Reads: 216

```
Hi,

thank you for letting me know. Seems like the "shipped" which means that the order is packed and a pickup is scheduled got to the customer but the message I sent separately once I received tracking did not go through. I just fixed it so I will resend the messages.

Thank you again, Martin. :)
```

---
## \#195 Posted by: Martinsp Posted at: 2019-02-23T11:40:15.277Z Reads: 222

```
Hi,
not sure why the other thread about power consumption when the switch (any antispark) is OFF was closed but here are the measurements I promised
Just a quick measurement nothing fancy. The input voltage was 56V and the current consumption was 2mA which is 0.112W. I consider this pretty low, example: 10S 10Ah battery (420Wh) would be drained in 3750 hours which is around 156 days so almost half a year of the battery sitting. 
You may consider this somewhat quick, the reason why I personally dont think so is that I can not imagine having a complete board (battery, switch and something on the output VESC etc...) sitting for half a year without me taking a look at what state of charge it is at least once or twice in the 5 months. 
![IMG_20190223_121058|375x500](upload://ydRUY4Ial48aRzPTL3VaVuBdUqM.jpeg) 
![IMG_20190223_121136|666x500](upload://4Ya7QDeDrdCFMx5fgqgkHvwk0js.jpeg)
```

---
## \#196 Posted by: mutantbass Posted at: 2019-02-23T11:50:30.836Z Reads: 200

```
Hey @Martinsp is this also the same for the regular anti spark switch without the push to start?
```

---
## \#197 Posted by: Martinsp Posted at: 2019-02-23T11:57:17.751Z Reads: 197

```
Yes I have just added a link to it in the thread for the regular AS switch
```

---
## \#198 Posted by: b264 Posted at: 2019-02-23T21:17:55.786Z Reads: 199

```
I can definitely envision that scenario if you made a new cooler board and you have like 5 boards and you just haven't grabbed that one in a long time when you grab a board to ride.

It's probably more common than you think.
```

---
## \#199 Posted by: CarbonV Posted at: 2019-02-25T08:31:26.363Z Reads: 192

```
Would you mind checking my pm again? :slight_smile:
```

---
## \#200 Posted by: nuttyjeff Posted at: 2019-02-25T12:02:11.351Z Reads: 203

```
[quote="Martinsp, post:195, topic:60879"]
The input voltage was 56V and the current consumption was 2mA which is 0.112W. I consider this pretty low, example: 10S 10Ah battery (420Wh) would be drained in 3750 hours which is around 156 days so almost half a year of the battery sitting.
[/quote]

Thanks for taking the time to help the do your tests!

I have 2 comments on this.

* A 420wh battery at full charge will indeed take 156 days to drain from 100% to 0, which is completely acceptable imho. (However, i think the wh of a battery is calculated by its nominal voltage, not its max voltage, making a 10s10ah battery either 360wh or 370wh depending if its a liion or lipo, but im just nitpicking). 

* A note on the website to indicate this drain would be useful to those who are unaware. I could see the possibility of someone using your switch on a smaller battery pack, say a 7s6ah, and leaving it at 60% charge. That'll drain to 0 in a month.

Also, just wondering if there was any way to get the passive power consumption even lower to that of a Unity (9uA)?
```

---
## \#201 Posted by: The_Dude Posted at: 2019-02-25T14:11:35.729Z Reads: 197

```
Hi @Martinsp,
I have some problems getting my &quot;push to start anti spark switch with pushbutton&quot; to work and probably need some help. 
So far I connected everything including the 2 phase sensing wires to the motor leads. I am able to complete step 3.1 of the instructions successfully (potentiometer in end position, setup LED is ON) :grinning:. 

Then I plug in my VESC, your LED switch and the battery. VESC turns ON and also the green setup status LED is ON. But then, no matter how far I turn the poti clockwise, the VESC does never turn off as described in the manual :confused:. 
When I use a voltmeter instead of the VESC to check (sensing wires still connected to two motor leads) I am able to tune to the setting point where the voltage drops down to 0 Volt (switch OFF) and if I turn the wheel, the voltage goes back to battery voltage (switch ON). Then I push the LED button until the green LED starts to blink to finish calibration :thinking:.

Now the problem is still, that as soon as I plug in the VESC (instead of the voltmeter) and connect the battery, the VESC immediately powers on (at least the blue LED on my VESC is on) but I am no longer able to turn the VESC OFF with the LED switch - it just stays on and does not go off (the switch LED is also on, all the time). Furthermore there is no power throughput - the blue power LED of the VESC is still on, but even if I pull the gas pedal, the motor does not turn, only a quiet whining sound. Just to mention, when I plug in the battery directly to the VESC everything works fine.

Sorry for the lengthy explanation, I just wanted to be as precise as possible :sunglasses:.
```

---
## \#202 Posted by: Surfer Posted at: 2019-02-25T14:27:49.054Z Reads: 181

```
Gently turn the screwdriver clockwise to increase the time, counter-clockwise to decrease the time  :)
```

---
## \#203 Posted by: The_Dude Posted at: 2019-02-25T14:33:44.015Z Reads: 187

```
Thanks, but this is what I mentioned with "I am able to tune to the setting point" - but it has absolutely no effect with the VESC connected, only works when using a voltmeter instead of the VESC (the VESC is totally ok, I checked this).
```

---
## \#204 Posted by: Martinsp Posted at: 2019-02-25T16:19:04.487Z Reads: 187

```
I think you contacted the customer service as well right? Just to avoid confusion and keep it in one place. I have just replied to the email with the same message as you posted so I think it is you.
```

---
## \#205 Posted by: The_Dude Posted at: 2019-02-25T16:32:29.971Z Reads: 190

```
Yes, sorry - didn't know what you prefer. So I tried both way's. Is it ok if for you I use the customer service/email until we find a solution and then I will post the solution here (may be it's of interest for the other user on the forum).
```

---
## \#206 Posted by: rusins Posted at: 2019-03-06T15:12:53.455Z Reads: 193

```
Hi @Martinsp! Just received your push to start switch today! (shipping was exactly 1 week, nice!)

Was wondering if it would be safe to drive my board's front and rear 12V LED lights from the 12V source on your switch. The small LEDs are rated to 30mA I believe, and seems like they are wired up in a 3s4p configuration on each end (with some resistors too, so actual current is probably smaller), so total max current draw would be 8 * 30mA = 240mA. Would that be too much, or can I safely do that? :slight_smile:

Edit: If I hadn't broken my own 12V DC source I could just measure the current flowing through them, but here I am looking up LED datasheets :man_facepalming:
```

---
## \#207 Posted by: rusins Posted at: 2019-03-11T01:30:28.544Z Reads: 179

```
My beefy 12V converters arrived early in the mail, measured two of my white LED lights, and the current slowly rises as they heat up, but I think it should stay below 150mA. Can the push to start switch handle that @Martinsp ? Then again, I found out that less powerful 12V converters are quite small and cheap, so I'll probably get one of those just to be safe.
```

---
## \#208 Posted by: Jansen Posted at: 2019-03-16T04:53:56.575Z Reads: 174

```
[quote="The_Dude, post:203, topic:60879"]
but this is what I mentioned with “I am able to tune to the setting point”
[/quote]

I am having this same issue right now and can't get it figured out.... what did you do @The_Dude or @Martinsp can you help me out....
```

---
## \#209 Posted by: The_Dude Posted at: 2019-03-17T19:19:28.994Z Reads: 177

```
Hi @Jansen,
unfortunately the push to start feature still does not work for me/my configuration (eBike MAC Motor) although I finally made it to tune the setting point. It took me quite a while but if you turn the potentiometer really slow and only in small steps (half a revolution each) and wait for a short while after each half-turn you find the spot when the (V)ESC goes OFF.  Sometimes, even at this point, I was not able to store the configuration by pressing the switch button several seconds. I had to turn the potentiometer a quarter or half turn further to get the green LED blinking.

With this configuration I am able to turn ON the auto switch by turning the wheel but the switch does not stay ON when I start driving. If I pull the throttle (using ADC mode of the VESC) the wheel starts spinning for one second or less and then stops - not enough power transmitted to the wheel, (V)ESC goes kind of OFF (blue LED is on but no power throughput). Interesting is, that I hear a "whining" of the motor when I pull the throttle again. Seems that there is some power transmitted but not enough the get the wheel spinning? After some tries, the auto switch bricks so that I even cannot turn it OFF or ON using the LED switch. Last exit is disconnecting the battery. I have two auto switches, both of them show the same behavior, so it seems to be symptomatically and not a defect switch. 

Interesting thing ist that at one (only) point in time it worked quite good but after I put the auto switch to another location in the casing it stopped working again. Maybe the auto switch is sensible to any kind of interference, but I don't know.

I described the situation to @Martinsp in detail and offered him to take some measurements (with his guidance) to assist in finding a solution. Last time was more than 2 weeks ago, I am still waiting for his reply. I would be really happy if I could get this push to start switch working since I really like the feature - but it's simply not working reliably.

Any help of the forum is highly appreciated! Would be happy to know if anyone got it working.
```

---
## \#210 Posted by: sayekim Posted at: 2019-03-17T23:37:15.958Z Reads: 162

```
Yeah I got the same problem with the new switch. I can get it as far as to configure the turn on point but it doesn’t stay on. When I magically do get it to stay on and finish the setting and then try the roll to switch it on, it immediately switches off again after I hit the throttle. 

I was on contact with @Martinsp and he offered to replace mine if I send this one back. I was okay with that and now two weeks further I have still yet to hear from him where to send it to.
```

---
## \#211 Posted by: The_Dude Posted at: 2019-03-17T23:49:15.877Z Reads: 166

```
Thanks for your comment. I think a replacement of the switch won't help since both of my switches have the same issue too. Would be good if @Martinsp could come up with a proposal how to solve the issue with his switches. Actually I would be better (and cheaper) with a simple ON/OFF anti-spark switch.
```

---
## \#212 Posted by: Jansen Posted at: 2019-03-18T05:40:20.736Z Reads: 174

```
@sayekim @The_Dude ok so I am not the only one then.... I thought maybe I had a bad solder joint or something but mine is pretty much all the things you talked about @The_Dude Before I saw your comment I actually did get it finally to do the blinking green light and the push to star feature working basically by turning the potentiometer super slow till I see it switch over, but everything else is super unreliable and doesn't work. Sometime the auto-off feature will work after like 5 minutes, sometimes it doesn't turn off at all on its own, a couple of times it has turned off in less than a minute. Sometimes the button works to turn it on/off, sometimes it doesn't. Then I've had times where the push to stat works, i give it a little throttle and it seems ok, then I give it throttle again and nothing until I restart my board and/or remote. I also seem to be lacking power when it is working but I think that may be a VESC or remote setting, but maybe not. Yeah hoping @Martinsp has an idea on what to do or what;s going on cause this is my 2nd switch from him as well that is having issues and I really want to take advantage of it and the features but it's been more of a pain so far.... sucks. Any suggestions for us @Martinsp??? Did you test the switches before they were sent out and were they working ok or do they get sent just once they are put together without any testing out of curiosity? Welcome any feedback/thoughts/suggestions from anyone on the form.

Thanks
```

---
## \#213 Posted by: The_Dude Posted at: 2019-03-18T06:04:52.186Z Reads: 172

```
Seems we're all in the same boat. I also hat the thought that the "lack of power" might be a VESC thing. So I tried running the identical setup without the push to start switch (XT90 anti spark plug, old school). With this setup I have non issue at all, absolutely reliable! I am quite sure, that at least in my case, this behavior is only due to the push to start switch.
```

---
## \#214 Posted by: Jansen Posted at: 2019-03-18T06:21:31.860Z Reads: 176

```
[quote="The_Dude, post:213, topic:60879"]
I am quite sure, that at least in my case, this behavior is only due to the push to start switch.
[/quote]

Hmmmmmm..... ok. That's really good to know. Thanks for that, I will do the same thing and try my set up with a different switch to see if that changes anything for me.

Thanks again! Keep me posted on anything you figure/find out and I will do the same.
```

---
## \#215 Posted by: The_Dude Posted at: 2019-03-19T22:19:10.499Z Reads: 166

```
Hi @Martinsp, I'm still waiting for a short notice from your side. I will wait till weekend for an answer - in case I get no response I will open an issue on Paypal since the product I bought does not work as expected and therefore does not match the description in your shop.
```

---
## \#216 Posted by: sayekim Posted at: 2019-03-24T22:41:07.861Z Reads: 169

```
So what is going on here? He was responsive a month ago and now he’s gone. 

I’m stuck with a faulty push to start from the new batch @Martinsp

I have a hard time believing he’s taken off and won’t come back since he does esc repairs and supplies @hyperIon1 with antispark too.
```

---
## \#217 Posted by: Superflim Posted at: 2019-03-24T22:44:12.899Z Reads: 169

```
He isn’t responding to me either....
```

---
## \#218 Posted by: goldrabe Posted at: 2019-03-25T00:16:30.354Z Reads: 173

```
@sayekim @Superflim have you guys tried his chat on the website? 
He was responsive on that channel.

http://sprusi.com/index.php
```

---
## \#219 Posted by: Jansen Posted at: 2019-03-25T11:00:05.689Z Reads: 174

```
Dido here... sucks
```

---
## \#220 Posted by: Martinsp Posted at: 2019-03-26T17:28:29.559Z Reads: 185

```
Hello everyone,

sorry for not responding but I have too many PMs to respond to and it is just overwhelming. Plus personal life, the shop is not my main source of income I have a "normal" day job so the time really is tight :confused:
 
If you dont mind I would like to tackle the problems (switch issue, shipping issues and lost packages etc...) one by one. 
I was finally able to reproduce the issue some people described and it turns out that the passive components used in the switch made it not possible to operate as it should on some systems. Two customers that were experiencing this issue had the same motor so I bought it, thats how I figured out what the issue was/is. Also that is the reason I did not find out earlier. I think it happened because I was trying to make the switch work on as many systems as possible (eboards ebikes escooters...) and in the end it did not work out quite so well, not enough optimization.

So what will I do about this? I am rushing manufacturing of new units that you (the ones affected) will get as a free replacement unit. I will need you to send me a PM as follows please use this title so I can easily find it and sort out "PTS v7 01/19- (your name)" in the message I would like you to put your situation so what setup you use (battery, BMS or not, what VESC/ESC, motor size and kv, what mode of the switch you tried) and please tell me about the setup process if it all went well according to instructions and what the switch does/does not do. If you dont mind making a short video demonstrating the behavior (nothing fancy I dont need you to talk or anything just show what is going on please).

I understand that I am asking for a lot but I am hoping to solve this once and for all, I could buy a bunch of motors and ESCs but that would just get too expensive really. 

With this information from you I will make necessary changes to solve the issues and get the new V8 manufactured and in your hands ASAP.

I really appreciate your patience and understanding, I will do my best to satisfy you all.
Martin.
```

---
## \#221 Posted by: SeanHacker Posted at: 2019-03-31T16:27:49.200Z Reads: 174

```
My switch went out (won't turn on) after 100 miles or so.
```

---
## \#222 Posted by: M.Hboards Posted at: 2019-04-04T16:41:35.150Z Reads: 168

```
Hey @Martinsp  I'm really sorry to put this statement out in public but i feel i have to do it to get a response. I understand you have a lot of pm's to sort through but i sent you a pm 17 days ago asking for the tracking number for a order i placed on you site and i have sill gotten no response. I have followed up with you multiple times just in case you missed my past pm's however I still got no response. I was really hesitant about putting this up here but I feel i gave you plenty of time (17days) to respond to my pm's or to responed to me via your sites contact us form. I currently have no proof my item was shipped and i really need it as is the final piece to my build. If this is not sorted out in a timely fashion I'm afraid i will have to file a dispute with PayPal.
(Please don't take this as a threat. I really don't want to ruin your reputation but i have waited over 2 weeks for a response and still haven't got one.)
```

---
## \#223 Posted by: sayekim Posted at: 2019-04-05T10:20:27.186Z Reads: 168

```
He is just one person doing all this so I am giving him a ton of slack. It seems he messed up with the last antispark push to start and is working on a new version that works for all of us. 

If you can’t wait I suggest you make yourself a loop key or do the chargeback or better ask for a refund because I am convinced he is good for all orders. He just needs to correct the mistake which seems to take time. 

I guess you can order the fatboy antispark which I believe has roll to start too. 

Oh by the way roll to start is nice but you should be aware that it slowly drains the battery. 
I’m not really sure but I think it was almost a 1 volt drop after not using it for a week. 

I’ll let you know Sunday how much it has dropped for sure.
```

---
## \#224 Posted by: sayekim Posted at: 2019-04-06T23:08:50.583Z Reads: 170

```
It was fully charged to 50.4 volts on Sunday last week and today Sunday they measured 49.6 and 49.7 volts. So not quite a 1 volt drop but 0.7 volts in one week from a fully charged battery in 12s6p configuration. 

![image|281x499](upload://t3ZgztbVzuIHhUvQfzh6AsH7Yo5.png) ![image|375x500](upload://fxumaPQ206euxZLh2xe6JYHtO1E.jpeg)
```

---
## \#225 Posted by: The_Dude Posted at: 2019-04-08T19:34:48.783Z Reads: 167

```
**PTS v7 01/19 - Dude**

Hi @Martinsp, here is my situation. I also send you a PM (Header is "PTS v7 01/19 - Dude") with my postal address.

1. Setup: 
12s-LiPo, no BMS, a MAC eBike Hub motor (5:1 planetary geared, freewheel, 1600 rpm (motor)/320rpm (wheel) at 48V, 16 pair pole, http://www.macmotortech.com/ebike-hub-motor.html). VESC6 with an ebike throttle connected to the ADC pins of the VESC used in ADC mode). 

2.   Commissioning: I made it to tune the setting point where the VESC goes OFF when I slowly turn the potentiometer. Sometimes, even at this point, I was not able to store the configuration by pressing the switch button several seconds. I had to turn the potentiometer a quarter or half turn further to get the green LED blinking.

3. With this configuration I am able to turn ON the auto switch by turning the wheel but the switch does not stay ON when I start driving. If I pull the throttle (using ADC mode of the VESC) the wheel starts spinning for one second or less and then stops - not enough power transmitted to the wheel, VESC goes kind of OFF (blue LED is on but no power throughput). After pulling the throttle several times more, the auto switch bricks so that I even cannot turn it OFF or ON using the LED switch. Last exit is disconnecting the battery. 

@Martinsp if you need further information please let me know!
```

---
## \#226 Posted by: M.Hboards Posted at: 2019-04-09T16:15:50.560Z Reads: 154

```
@SeanHacker just curious do you remember how long it took for you to get your switch when you ordered it and what shipping company delivered it?
```

---
## \#227 Posted by: SeanHacker Posted at: 2019-04-09T16:51:30.407Z Reads: 152

```
I can't really remember. I'm pretty sure it took at least a week or two and it cam usps. I'm pretty sure I had to sign for it too.
```

---
## \#228 Posted by: M.Hboards Posted at: 2019-04-09T17:29:58.597Z Reads: 152

```
Have you gotton a response from Martin regarding your broken switch?
```

---
## \#229 Posted by: SeanHacker Posted at: 2019-04-09T17:30:29.523Z Reads: 155

```
Nope. But I've only posted that it broke here. Just haven't had the time to deal with it yet.
```

---
## \#230 Posted by: sebaszz Posted at: 2019-04-10T16:51:47.529Z Reads: 155

```
1 week past, no shipping info received

really not happy with this service. If you do not have the time to supply your customers. Put your orders on hold instead of accepting new ones.
```

---
## \#231 Posted by: Shaz Posted at: 2019-04-11T07:53:31.457Z Reads: 147

```
Can someone share the wiring diagram instructions? I lost the instructions that came with the package.
```

---
## \#232 Posted by: Superflim Posted at: 2019-04-11T07:54:10.576Z Reads: 146

```
It's on the website too
```

---
## \#233 Posted by: sayekim Posted at: 2019-04-11T09:16:55.866Z Reads: 149

```
From a business perspective I believe it is just more favorable to keep accepting orders. Understandably. 

Stating anything about delays is bad for your business. 

However if I’m making enough money 💰 I’d do it anyways and take my losses.
```

---
## \#234 Posted by: Shaz Posted at: 2019-04-11T17:11:46.230Z Reads: 143

```
Doesnt show which way the battery input is and which way to the vescs
```

---
## \#235 Posted by: ervinelin Posted at: 2019-04-11T19:28:05.883Z Reads: 148

```
From my understanding the switch itself draws some current even when it is off. I raised this issue some time ago in the forum and no one seemed to think that it's a critical issue....

I had one 10S2P pack drain to zero from just leaving it unattended for a few weeks. Have since swapped to a loopkey on that deck.

Note that the older style antispark did not have this issue... Something about having some control circuitry onboard which causes the current draw.
```

---
## \#236 Posted by: sayekim Posted at: 2019-04-11T19:45:09.341Z Reads: 139

```
I’m running the older one and it was my understanding that these roll to start all have current draw.
```

---
## \#237 Posted by: lazarus Posted at: 2019-04-11T21:50:55.110Z Reads: 140

```
Depending on the design of the board it is possible to get the draw down to uA, effectively nothing. A single cell could power it for years. Did someone test the current drawn by this switch?
```

---
## \#238 Posted by: ervinelin Posted at: 2019-04-12T00:20:33.248Z Reads: 145

```
Yes someone did (but not if this particular anitispark), it's significant enough to drain your pack enough to notice.

My non push to start also had this issue.
```

---
## \#239 Posted by: lazarus Posted at: 2019-04-12T00:29:28.208Z Reads: 150

```
Thread is too big to search effectively but I did find [this post](https://www.electric-skateboard.builders/t/push-to-start-switch-out-now/60879/195) above. 2mA * 57V is pretty thirsty, understandable for someone to decide either way.

Wonder what the Unity's passive draw is, do you know off hand @Deodand?
```

---
## \#240 Posted by: ervinelin Posted at: 2019-04-12T00:51:45.807Z Reads: 152

```
I think I had friends who checked. It's next to nothing on the unity.

And yes the draw on these newer push to start antisparks is not insignificant. The argument by some manufacturers was that there is no way to do it without some active circuitry. Some users claimed you should always keep your board juiced up ready to go. Others say the BMS should kick in to prevent over drawing the pack.

IMO, this should have been information given upfront. That the switch does draw current even when turned off. Would have saved my pack from being drawn to zero.
```

---
## \#241 Posted by: Deodand Posted at: 2019-04-12T01:49:32.508Z Reads: 153

```
The unities passive current draw is around 9 uA which is small enough that even if almost fully discharged battery it would take a few years to kill.
```

---
## \#242 Posted by: lazarus Posted at: 2019-04-12T01:59:38.956Z Reads: 148

```
Nice, that's lower than the voltage regulator in my remote. :grimacing:
```

---
## \#243 Posted by: rusins Posted at: 2019-04-14T23:48:49.652Z Reads: 155

```
Question for people who have the new version: did you have any trouble getting the switch into setup mode? It's step 3.1 in the instruction manual, where you need to have the switch on the left, and potentiometer all the way back counterclockwise where you can hear it clicking, which should make the green LED onboard turn on.

I followed the instructions and managed to get the green LED to turn on, but after a few seconds it went out, and now I can't get it to turn back on again. I've tried nearly any combination imaginable: toggling the switch and turning the potentiometer clockwise, attaching battery, then going left and counterclockwise again, trying to turn counterclockwise a bit after the clicks and attaching battery, detaching the ESC while performing steps, etc. Tried everything, cannot get the green light to turn on again for the life of me. Any help would be much appreciated, I want to set the switch up to see if I get the same problem (with the switch staying on after pushing) others have been having or not.
```

---
## \#244 Posted by: sayekim Posted at: 2019-04-15T06:28:07.361Z Reads: 155

```
The way it should work is turn counter clockwise until you hear click then connect battery. Repeat until you see the light. 

I’m waiting for the replacement. Unfortunately mine just doesn’t want to stay on with throttle input. 
Running the old one in the meantime which I required from another member here. I used to have on of the old ones before myself but that one blew during a hard acceleration on a ride.
```

---
## \#245 Posted by: The_Dude Posted at: 2019-04-26T21:24:33.881Z Reads: 147

```
Hi @Martinsp, can you give us an update on the status. Last time we heard from you was a month ago. 
Did you get the push to start feature working? Actually I'm also concerned about the power drawn when the switch is off, are you also working on that?
```

---
## \#246 Posted by: The_Dude Posted at: 2019-04-29T19:39:04.092Z Reads: 141

```
Hi, has anyone already got an answer from SPRUSI? Slowly but surely my patience comes to an end, flow of information has completely broken down, no response since several weeks  ... @Martinsp please take my question serious, trust of current and potential new customers is easily lost!
```

---
## \#247 Posted by: sayekim Posted at: 2019-04-29T20:01:47.812Z Reads: 142

```
Nada dude. 

Last thing was send him a pm and he would sort it out for all of us. 

That was too long ago for me to bother to check when it was. 

@Martinsp time to tell us you ducked up royally or to send us a working one asap as in now.
```

---
## \#248 Posted by: Jamie42 Posted at: 2019-04-29T21:17:36.445Z Reads: 140

```
Ordered a switch from @Martinsp 1.5 weeks ago which should've been delivered already... No response either.
```

---
## \#249 Posted by: sebaszz Posted at: 2019-04-30T14:17:14.009Z Reads: 141

```
opened paypal dispute 2 weeks ago. No response. Now escalated to paypal.
```

---
## \#250 Posted by: Jamie42 Posted at: 2019-05-05T13:21:51.887Z Reads: 136

```
Still nothing. I am going to wait for 1/2 more weeks since I really want that switch. If I don't get a response by that time I will try a dispute.
```

---
## \#251 Posted by: Martinsp Posted at: 2019-05-05T18:07:02.716Z Reads: 136

```
Hello everyone,

I am sorry (I know it is not enough) for the ridiculous time it takes me to get back to all of you. I still have lots of PMs unanswered because I just cant keep up.

Anyway, I have been through 3 new iterations of the switch which did improve a lot but since this mistake I dont want to release another version uitil I am 100% sure it will work for everyone. I will reply to all of you that sent me a message/reply to this: 

[quote="Martinsp, post:220, topic:60879"]
...“PTS v7 01/19- (your name)”...
[/quote]

and offer you a refund on the full amount. 

**As for the new version, there are pretty radical changes. There will no longer be any sense wires, the sensing of motor rotation / ESC activity will be done through the power wires and there will be no setup procedure, it will be all automated with some minimal user intervention like spinning the motor** 

I have unfortunately broken my hub motor so I will have to get a new one (if you have one for sale in EU let me know please! :slight_smile:) so this extends the time and I just felt like it is too much even for my standards of (not)sticking to schedules and promising dates which turn out to not be achievable. That, apart from extending my testing equipment is something I have to work on.

Anyway, expect a reply from me and enjoy the rest of your weekend!
BR, Martin.
```

---
## \#252 Posted by: banjaxxed Posted at: 2019-05-05T21:35:48.884Z Reads: 130

```
Hey Martin, I’ve still got your switch with sensor wires but happy to return and go with a newer model when ready

I have other switches to use if I manage to complete that build before you’re ready with a new version, is that something that would be ok?

Props for the above, that is a painful product support
```

---
## \#253 Posted by: sayekim Posted at: 2019-05-06T06:36:12.485Z Reads: 125

```
Good update. 

I want this new version. Will it be a month or longer before it's released?
I'd be happy to test it.
```

---
## \#254 Posted by: 702vegas Posted at: 2019-05-06T21:08:44.106Z Reads: 124

```
Should i not bother installing the one i have right now?
```

---
## \#255 Posted by: rusins Posted at: 2019-05-06T22:17:34.387Z Reads: 128

```
I mean unless you're short on time I don't see why not, surely the current switch must work for some motor configurations.

Update from my part: my brother has tried setting up his push to start switch every day now for the past week with no luck (setup LED won't ever turn on), will try to tinker with it myself when I see him in 3 weeks, but looking pretty grim :confused: I'm glad the setup procedure will be changed for the new model, whenever that comes out.
```

---
## \#256 Posted by: Jamie42 Posted at: 2019-05-12T10:02:54.273Z Reads: 125

```
This looks good. What will happen to poeple like me that bought a V7 but did not get it sent? Do you have some kind of estimate when a reliable version will be available?

Edit: Also, why does your switch still show as in stock when you don't send 'em out?
```

---
## \#257 Posted by: snwmelt Posted at: 2019-05-22T11:10:27.390Z Reads: 120

```
I ordered the V7 switch from your site yesterday, will I be receiving the updated one instead?
```

---
## \#259 Posted by: Martinsp Posted at: 2019-06-09T19:42:59.376Z Reads: 102

```
Hi,

Im sorry about this but I dont think I have received any emails/messages that you have not received a refund.

I think we all know by now that Im juggling time here as much as I can I am sorry I really can not keep up with the messages at least not now. The only reason I reply to PayPal right away is because I really can not afford getting it taken down so I stop whatever I am doing to reply. I am sorry I dont do this every time someone messages me here or on my website, I would not get anything done that way and well it is a "one man show" I dont have any customer service team or something like that.

I have also acknowledged that I made a mistake during the design of V7 and I have done my best to fix this. I have manually refunded everyone as far as I know, If you have for whatever reason not received your money contacting me would solve this issue. I do check the email notification on my phone I see the messages if it is something like this I do reply as I can. 

Im not sure what you mean by fake, this is the first time this has happened to me (large product issue/recall) apart from this my products worked unless handled incorrectly and if it was not possible to determine the cause of a fault I refunded money to customer or sent a new unit. I really dont know what you mean by fake.

I am definitely not here to rip someone off.

So bottom line, message me (I have not seen a PM from you regarding this) and I will get this sorted our for sure.

Im sorry again, I truly do what I can and realize it is not enough I only have 24 hours a day, Martin.
```

---
## \#260 Posted by: Martinsp Posted at: 2019-06-09T19:46:58.437Z Reads: 92

```
The switches that can be purchased now have a firmware fix for this issue. Im waiting for some parts to test some last things for V8 as well as other products to get them manufactured at the same time
```

---
## \#261 Posted by: The_Dude Posted at: 2019-06-10T07:11:34.042Z Reads: 96

```
@Martinsp look at your PM here in the forum:

![50|596x500](upload://8jLARs7RAEtloXcHMT4EJXsu1sp.jpeg)
```

---
## \#262 Posted by: Komamtb Posted at: 2019-06-10T10:42:55.277Z Reads: 92

```
Hey @Martinsp I just bought a V7 a few days ago, for the first generation one, you have them in stock and ready to ship?
```

---
## \#263 Posted by: Jansen Posted at: 2019-06-10T17:14:30.927Z Reads: 93

```
I feel the same way and have PM'd you at least 4-5x's over the past month or two since you haven't sent the refund or responded to my original PM sent to you per your request with the title and subject info you asked for. Please send my refund for the smart switch to my paypal which you can get to using my email which is JansenFalvai@gmail.com. Can I expect this to get done today hopefully since it's been months since promising to take care of this? Thanks in advance for your help on resolving this matter. @Martinsp
```

---
## \#264 Posted by: Martinsp Posted at: 2019-06-10T17:35:49.243Z Reads: 95

```
@The_Dude Just sent the money back. Sorry again. @Jansen Your payment is not refundable thats probably why it was not refunded. I just sent you the money regularly as friends and family. I hope everyone has their money back now.

@Komamtb They are not in stock anymore I dont think, maybe one or two. But if you are asking if you receive the fixed one then yes, it wont have this issue.
```

---
## \#265 Posted by: pjotr47 Posted at: 2019-06-10T17:38:13.068Z Reads: 98

```
@Martinsp

You have a pm from me.
```

---
## \#266 Posted by: Jansen Posted at: 2019-06-12T19:05:50.626Z Reads: 101

```
You're awesome! Thanks @Martinsp really appreciate you taking care of that and sorry again it didn't work out as planned. Good for you for taking responsibility over it though. Shows true colors. I will still be a customer buying the next version you have that proves to be tested and working right. Best of luck my dude!
```

---
## \#267 Posted by: Komamtb Posted at: 2019-06-12T20:48:36.512Z Reads: 101

```
I'm really excited to test a new one, the first gen one was all beaten up, but worked without any issues, it was the best investment in my board.
```

---
## \#268 Posted by: Martinsp Posted at: 2019-06-24T05:10:17.599Z Reads: 97

```
@Jansen @Komamtb  Thank you very much for the kind words, this kind of feedback keeps me going! Now I just have to eliminate the bad feedback haha

**UPDATES:** I have received the prototype units that I needed to prove that the new way of sensing if the motor is rotating is working the way it should not only in theory but in the real world. However there still has to be changes made because on high kv motors the sensing is not precise enough, so there has to be one more version, the final one. And that is the reason for this update. 

I would like to make this project more open and more guided by the community. It started as a project of my own for my board so I made it the way I thought was the best. Now since I am offering it to you I think you should be the ones setting the goals. So here is a list of my goals and improvements from the last version:

* Improve current handling capability
* P channel / high side switching to allow for sensing without sensor wires.
* Adjustable threshold to make sure the switch works with all motor and battery combinations
* Compact
* Make the firmware entirely in Arduino IDE to allow for easier firmware update by user
* USB connection to update firmware and adjust settings more precisely and without hardware potentiometer
* Lower power use when not active

So that is the list as of now. If you have any idea you would like to see let me know I will see what I can do! :) 

I just got back to the forum after a few days (if you messaged me, Im going to reply to you shortly) and recently discovered there is a new news forum :O I have to check that out and soon you will find me there as well! :) 

**BTW:** I have a new product coming out shortly Im very excited about it. It is something I miss ever since building my first battery a couple of years ago. I think you will like it! :) What I need is and app, but I unfortunately lack the knowledge/skill to create a reliable one from scratch. If this is something you can do let me know in a PM please (subject "APP development"). The app pretty much needs to connect to a device via bluetooth and display some string that the device send and send some strings back to adjust some parameters in the device itself. I may make a thread about this in a few days.

That will be it for now, I want to give some more frequent updates and interact with you more. I need to organize my time better for it. Im working on it, slowly but surely.

Have a nice day everyone! 
BR, Martin.
```

---
## \#269 Posted by: Gamer43 Posted at: 2019-06-24T06:28:36.124Z Reads: 82

```
~~I really shouldn't be helping my competition~~


@Martinsp 
Check out the LTC7004 and LTC7001 for high side N-Channel MOSFET driving, they look expensive but are literally half the cost at 100 quantity. LTC7004 is rated for 60V, LTC7001 is rated for 100V.

Run an Attiny85 at 1MHz; NCP781 has very low quiescent current. If you want to go all out with a buck converter, the LM5165 requires minimal external components and features 10.5 uA quiescent current. 
If you want to make it configurable/reprogrammable, 8-DIP socket :).  

For auto-turn off, you can use something like the INA181 and a current shunt to detect activity on the power rails. This also allows for user programmable over-current limits. 

I made a smart antispark that has roll-to-start and auto-turn-off. I rode it around for an hour on a 12s4p 50% charged battery, single 6355 TB 4.12 VESC board with the auto-turn-off threshold set to ~8-10 minutes. Roll-to-start works every time, I don't even have a push button on the thing.

I could not get auto-turn-off to work on my ~~damaged~~ DiY 4.12 VESC, the inductor is kind of broken, so that is probably messing with the current draw of the VESC.
```

---
## \#270 Posted by: Martinsp Posted at: 2019-06-24T06:57:11.927Z Reads: 82

```
@Gamer43 Thank you for the feedback!
I am planning on using P channel mosfet, this way I avoid the gate driver. For sensing, the spike or change rather gets up to 2-3v with hub motors and about half that with belt driven systems (keep in mind that I am doing this with the same rotor speed not ground speed/rpm) so the sensing is pretty stable. 

Attiny85 unfortunately has too few IO for the features even of the old version. I use a 32 pin IC which is just too big in removable DIP package so using a usb makes more sense in this case at least from my point of view.

Thank you for the input anyway I will consider it and take a closer look at the mosfets and gate drivers maybe use them if it proves to be a good way of moving forward
```

---
## \#271 Posted by: Gamer43 Posted at: 2019-06-24T06:58:42.736Z Reads: 83

```
Hold on a sec, how many features is this thing going to have? XD.
Also, if you opt not to use a gate driver, how will you handle precharge/in-rush current limiting? I've found that really big resistors (through-hole, or high power SMD) are needed for the precharge route.

I've also found that N-channel + gate driver can be cheaper than appropriately sized P-channel MOSFETs. P-channel MOSFETs are expensive X_X.

If you need a bigger chip, STM32L0 line features crystal-less USB and insanely low quiescent current draw.

I'd just like to add, I can hand spin a 190KV motor to trigger roll-to-start on my antispark xD. Although, if my math is right, a 270KV motor would only need the board to be rolling at 5 Km/h at common gear ratios.
```

---
## \#272 Posted by: Martinsp Posted at: 2019-06-24T07:18:25.238Z Reads: 90

```
It is going to have as many features as 8kb and approximately 28 IO allows haha 😀

Yeah, high voltage high current p channel mosfets are expensive unfortunately.

Yeah I'm spinning them by hand as a test as well. I use 70kv hub motor and 380kv regular motor to cover the range between them. With hub motorbs it is easy they generate  more voltage at the same rpm... Im thinking of using an opamp or maybe just a comparator to deal with this but then I loose partially with opamp and completely with a comparator to adjust the threshold so I have to explore these two a little more to maybe find a solid compromise
```

---
## \#273 Posted by: Gamer43 Posted at: 2019-06-24T07:24:17.657Z Reads: 95

```
You should be able to get away with the MCU's ADC and a voltage divider, the precision should be okay at 12-bit resolution.

Honestly, I don't see the benefit in being able to adjust the threshold, as I'm guessing most users just want the board to turn on when they kick it. 

My firmware takes up 1,400 bytes and uses three GPIOs, so you're going to have A LOT of room to play with to add fancy features xD. (This is with the ~~unnecessary~~ push button :P)

I handle the in-rush current problem with the RC network described in the LTC7004's datasheet. The MOSFET will explode at a large enough capacitance, but this capacitance is huge, like 10mF or larger. You'd have to be running 4wd 4.12 hardware to even get close.
```

---
## \#274 Posted by: Martinsp Posted at: 2019-06-24T07:33:49.405Z Reads: 103

```
The resolution of a standard ATxxx arduino compatible chip is 10bit but even that should be enough. 


Yeah I know that most people want to plug and play but with the diversity of people's builds, making it plug and play for everyone is just not possible. I am planning on implementing a self learning procedure to make this as straight forward as possible. It is not on the list of features at the moment because it needs some work before I can promise that it will be implemented in final version. 


With my regular switch and this push to start as well I test the hardware with close to 11000uF capacitor bank at 12S. That's without a dedicated mosfet driver and even without a heatsink. I still need to perfect it but it can switch the load without issues.
```

---
## \#275 Posted by: Martinsp Posted at: 2019-06-24T07:36:42.758Z Reads: 107

```
But the main goal to future is to increase voltage range rather then capacity of the load and precharge or other ways to protect the mosfet. It has been two or three versions since I had any issue with blown fets due to inrush
```

---
## \#276 Posted by: Gamer43 Posted at: 2019-06-24T07:43:45.372Z Reads: 106

```
N-channel with gate driver :).
```

---
## \#277 Posted by: Komamtb Posted at: 2019-07-21T16:41:00.684Z Reads: 95

```
Any updates? I'm now waiting for two of them.
```

---
## \#278 Posted by: Jamie42 Posted at: 2019-07-21T19:20:50.409Z Reads: 96

```
Here's the reason I opened a dispute (got my money back) and bought an anti-spark from 3Dservisas...
```

---
## \#279 Posted by: Komamtb Posted at: 2019-07-21T20:11:26.818Z Reads: 94

```
Oh, the battery draining one :smiley:
I've used Martins switch before and really liked it, so kinda want to continue doing it.
```

---
## \#280 Posted by: Jamie42 Posted at: 2019-07-25T11:47:46.650Z Reads: 84

```
I want Martins switch too, but I waited a long time without updates. So I ordered a switch from 3Dservisas and that one arrived the same week.
```

---
## \#281 Posted by: Komamtb Posted at: 2019-07-25T12:49:00.943Z Reads: 85

```
loads of my components are ariving, two builds rely on this swith, @Martinsp could you be kind and update us?
```

---
## \#282 Posted by: ArtFillin Posted at: 2019-07-29T21:22:33.381Z Reads: 80

```
About the timer personally I would wish that you can change it from never(maybe add a deducated butoin) 5min, 10min, 30min, 60min
```

---
## \#283 Posted by: Komamtb Posted at: 2019-08-19T08:59:17.479Z Reads: 66

```
Mine too patience have gone to the end and I bought 2 from a forum member, now, how do I get my money back? I have opened a dispute on paypal, but it's not showing any progres, opened it about 10 days ago, any tips?
```

---
## \#284 Posted by: Martinsp Posted at: 2019-08-19T09:13:17.878Z Reads: 64

```
Hi, sorry for this. The manufacturing has been postponed and orders stopped. I will end your dispute with refund asap. 

Regards Martin.
```

---
## \#285 Posted by: FredrikHems Posted at: 2019-08-19T10:39:34.518Z Reads: 66

```
Hello @Martinsp 
Could you please see the PM’s I have sent? 
Thank you.
```

---
## \#286 Posted by: Komamtb Posted at: 2019-08-19T14:24:17.159Z Reads: 59

```
Heey, @Martinsp I honestly feel bad about taking funds away from the future project, I was one of the first people to buy your first version switch and this for me is one of the best things, that came out, out  of this forum, the product itself is great, I'll sincerly wait for your future switch and buy a few directly if they ever come out.
```

---
