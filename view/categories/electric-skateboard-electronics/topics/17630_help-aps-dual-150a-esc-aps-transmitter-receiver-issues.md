# \[HELP\] APS Dual 150A ESC/APS Transmitter-Receiver Issues

### Replies: 50 Views: 2984

## \#1 Posted by: DaveMess Posted at: 2017-02-13T03:11:23.970Z Reads: 143

```
Looking for someone who has already set up this ESC. Here's my build in a nutshell:

APS Dual 150A ESC
APS 5065 motors, 270kV, 2200W, 60A (x2)
APS Transmitter/Receiver
8S Turnigy Lipo 5000mah (2 4s in series)
Enertion Dual drive kit (still on it's way, pending delivery on 2/13)


This is probably a simple issue, but I can't find a solution. I can't seem to get the transmitter/receiver to work with the ESC. 

I have the ESC plugged into CH2 on the receiver. Lipos are at a storage charge, 30.5V total. I power on the transmitter, then the ESC/receiver. I get 3 short beeps, a pause, and then it starts a pattern of 3 short beeps, pause, 3 short beeps, repeated 10 times. No response from throttle input, so I assume that the ESC isn't actually communicating properly with the receiver. I can't find any manual or information on what the beeping patterns actually mean. I have gotten it to do other patterns, don't remember how I made that happen, or what the beeps were. So does anyone know how to set this up properly? Do you have links for a more informative manual? Overall it seems the information for these ESCs is limited at best. 

Other information: Both ESCs are running CARLV_UV45. This isn't the firmware they came loaded with, I accidentally flashed one ESC to the wrong software during initial programming. I emailed Bruno and he told me to run this firmware instead, still not sure if it's the right one though based on the firmware version being 4.5 and the firmware the ESC came with was version 5.0. Also need your advice on this.
```

---
## \#2 Posted by: Davey Posted at: 2017-02-13T17:59:30.554Z Reads: 130

```
Hi Dave, I'll run the same setup. I haven't done it yet, but after my batteries charged fully (in a couple hours), everything should work. Here are some ideas of mine.

1.: Try to plug the ESC to CH1. I don't understand this manual completely but it might help: http://epowerhobby.com/wp-content/uploads/2016/08/APS-EVT3-DIGITAL-PROPORTIONAL-RADIO-CONTROL-SYSTEM-1.pdf

2.: Have you put the right amount of motor poles in your firmware of the ESC? I don't know if that changes something, but I would put the mark to the amount of the poles that your motor has. 

3.: There is also a pattern lexicon over here: http://alienpowersystem.com/wp-content/uploads/2013/06/Alien-ESC-Instruction-sensored-A5-USB-PDF.pdf

4.: In your way you did not press the "bind" button on the remote. The first manual explaines how to let the remote communicate with the ESC.

I will update this, 
Cheers, Dave
```

---
## \#3 Posted by: Davey Posted at: 2017-02-13T18:01:40.352Z Reads: 109

```
This is what might help: (please read manuals anyways)
 6- RECEIVER 
The Alien radio control system is supplied with RECEIVER.  
The products are matched by factory.  In case you need to BIND the system please follow this procedure: 
-Turn ON the Transmitter 
-Push the BIND button 
-Turn ON the Receiver 
The LED light will flash for few seconds. When the Light will be steady system is matched
```

---
## \#4 Posted by: DaveMess Posted at: 2017-02-13T19:02:35.596Z Reads: 99

```
Thank you for the manuals, I did have those ones. The ESC one didn't seem to correspond with our ESCs but I'll have another look. The program came with a motor timing of 3 in the software, not sure if that's right or not. Unfortunately I don't have my mounts still, snowstorm in the Northeast US held up my package I think. That or customs O.o I'll let you know if I get it figured out, let me know what software settings you end up using. I pretty much went with the preset values across the board for the CARLV_UV45 program. 

Edit: forgot to mention that the remote calls CH2 to be the momentary switch, while the receiver manual calls CH2 the throttle channel. They don't seem to match between the receiver and the transmitter. Trial and error shows that CH1 on the receiver must be the momentary switch, as when I plug the ESC into it and hit the switch, both motors go to full power. Press again they stop abruptly. Imagine my surprise when I did this the first time by accident...
```

---
## \#5 Posted by: Davey Posted at: 2017-02-13T19:33:17.503Z Reads: 87

```
My batteries are charged now. I have a 14 pole Turnigy motor and firstly I'll be using the HELI setup, because it supports 14 poles. I will load a better firmware on it when everything works, because HELI does not support breaking! I use a motor timing of 15, because I read that this one is a solid number.. Since I'm from Germany and I might not have got all your arguments correctly, I'm sorry for any mistakes in here.

Do you use a switch for your spare channel?

Edit: so I've got it right that the Acceleration-Trigger is CH1 on the remote, but CH2 on the receiver and the spare channel (CH2 on the remote, for LEDs and stuff) is CH1 on the receiver? this is so confusing, omg
```

---
## \#6 Posted by: Davey Posted at: 2017-02-13T20:07:19.816Z Reads: 79

```
Okay. I cabled everything together and the motor also des NOT spin, whether I plugged it in CH1 or CH2. But mine beeps in different patterns, but this might be caused because we have different motors
```

---
## \#7 Posted by: DaveMess Posted at: 2017-02-13T20:20:53.456Z Reads: 71

```
OK. I did see something about pulling the throttle to full power right after the first beep when you turn it on. See if that arms the ESC. It is incredibly confusing.
```

---
## \#8 Posted by: Davey Posted at: 2017-02-13T20:38:40.183Z Reads: 75

```
Oh yes it is. When I plug these together, I plug the ESC cable (Brown, red and orange) in the rx receiver. which way do you plug it? And there are some LEDs on top of the receiver. In my case, whatever I do, none of these turn on. My ESC (150A mini ESC BEC from Alien) should power the receiver, but there isn't a black cable and this confuses even more. I thought that I would not need an external battery if my integrated BEC (5V) powers the receiver.
```

---
## \#9 Posted by: DaveMess Posted at: 2017-02-13T21:06:13.389Z Reads: 76

```
OK that's basically where I'm at as well. The ESC cable should power the receiver according to the wiring diagram. I believe the proper connection is to have the ESC wire plugged into CH2. I forget which wire I figured out was the negative lead. I think it's the brown one. At the top of the plugs on the receiver you'll see a "+", a "-", and a third symbol. That third symbol represents the signal wire while the other two are for power. So put the brown wire in the negative side and see if your receiver powers up with a red light. Then try doing the full throttle thing and see what happens.
```

---
## \#10 Posted by: DaveMess Posted at: 2017-02-13T21:19:14.612Z Reads: 70

```
And now to top it off my delivery from Enertion went from delivery today to unscheduled delivery.. and it never made it to a UPS site in the USA so it's either stuck in customs or fell off the plane somewhere over the Pacific.. ugh -_-
```

---
## \#11 Posted by: Davey Posted at: 2017-02-14T17:07:56.800Z Reads: 63

```
So your motor spun once? I agree that the brown ESC wire is for the negative pole, the red one for positive and the orange one for signal. I found a wiring diagram for another ESC and that said this. My receiver does not power up with a red light. I'm building one with my friend and also his receiver does not power up. I will try it with more voltage since I'm using a 3S battery right now for testing and things (so if I plug something wrong nothing will blow up). I'll use my 6S batteries and maybe it works then. And I'm sorry for your package
```

---
## \#12 Posted by: DaveMess Posted at: 2017-02-14T17:20:07.929Z Reads: 56

```
I think it's weird that you're not getting a light on your receiver. We might have separate issues here unfortunately :confused:
```

---
## \#13 Posted by: Davey Posted at: 2017-02-14T19:17:08.032Z Reads: 51

```
Yeah I guess we're having different issues. Could you tell me the settings you put in the firmware and what voltage you are using? It's really annoying that the receiver(s) won't power on..
```

---
## \#14 Posted by: DaveMess Posted at: 2017-02-14T19:37:29.077Z Reads: 52

```
I was trying to run it at a full 8S. I did not change any settings from the default ones used for CARLV_UV45. What firmware did you download and install on the ESCs? Did you do the full setup described in the manual?
```

---
## \#15 Posted by: DaveMess Posted at: 2017-02-14T20:14:20.391Z Reads: 50

```
When you power on the ESC, see if you get about 5V across the + and - wires
```

---
## \#16 Posted by: Davey Posted at: 2017-02-14T20:56:49.960Z Reads: 50

```
nice, I'll try it with 6S later on. I used the HELI firmware (there is only one similar to this name) because it's the only setting where I could change the motor poles to 14. After I emailed Bruno (Alien support) he told me I do not have to change the motor poles in the firmware and it would also work if I use another firmware where 2-4poles is locked.
I don't know what you mean with the manual. I updated the firmware and changed some things like "cut off voltage" or "battery type" or "throttle acceleration" depending on my setup. 
Yeah, I think I'll measure it with a voltmeter tomorrow or so
```

---
## \#17 Posted by: DaveMess Posted at: 2017-02-14T21:08:46.411Z Reads: 51

```
Try it with the same firmware I mentioned above. With the HELI firmware you probably won't have brakes if I remember correctly. Oh and I guess you must have done the initial setup procedure as you have access to the ESC software. I was basically asking if you had changed the firmware at all yet, which you have.
Edit: the reason your receiver isn't powering on might be because the ESC Bruno builds for helicopters might not have a BEC, so there wouldn't be anything in the program to turn on the BEC and send power to your receiver. I know a lot of helicopter setups require you to have a separate BEC just to take the voltage from the batteries and take it down to 5V for the receiver.
```

---
## \#18 Posted by: Davey Posted at: 2017-02-15T15:42:31.511Z Reads: 54

```
Yeah I'll try out different firmwares. There is one called Sk... and I thinks it stands for Skate so I'll check this one out. What is the initial setup procedure? I know that there aren't any brakes with the HELI firmware, but it was the only one supporting 14 poles (now I know that every firmware does this so I can change it easily)
I have this ESC and it says that there is a 5V 3A BEC: http://alienpowersystem.com/shop/esc/alien-120a-2-7s-ev-mini-esc-bec/
I know that the ESC isn't the best one ever but for a poor student it should work :smile:
```

---
## \#19 Posted by: Davey Posted at: 2017-02-15T17:54:59.281Z Reads: 52

```
Oh thank you. I tried it with your firmware and the receiver powers on, 14poles and breaking is provided. Thanks!!!
```

---
## \#20 Posted by: DaveMess Posted at: 2017-02-15T18:16:26.673Z Reads: 51

```
Hey that's awesome! I'll give it another go when my drive kit comes, hopefully tomorrow. Send me a pic of your build! 😄
```

---
## \#21 Posted by: Davey Posted at: 2017-02-15T18:51:08.091Z Reads: 45

```
Oh man I'm so happy right now! Now it's just a couple of electronics laying on the floor, I need to buy/make an enclosure now. The motor spins very fine and I need to focus on the LEDs I want to install.
ATTENTION! Check that all wires are plugged in well and cannot get out. I plugged my wires and did not solder them because everything held together, but the Red motor cable slipped and there was a little wobble contact while the motor was running. This caused (of course) heat and the banana plug got hot and black (so the lication (the golden material) oxidized). The rotation of the motor was so strong, that my axle where the motor is mounted tilted and the cable got out.

I'll send you my build when it's finished. So what was your problem again? Should I send you some pictures of how I wired up everything?
```

---
## \#22 Posted by: Davey Posted at: 2017-02-15T18:52:22.564Z Reads: 37

```
Lesson learned: It's better to solder cables
```

---
## \#23 Posted by: DaveMess Posted at: 2017-02-15T19:25:08.926Z Reads: 35

```
Yeah just send me a pic of how you wired everything. I think I have it right but I don't have motor mounts yet so I can't really try turning it on again without wrecking my motors. Once I get them mounted it'll be safer to turn it on. Glad you got it working!!
```

---
## \#24 Posted by: Davey Posted at: 2017-02-15T20:23:13.085Z Reads: 38

```
Okay I'll send you a message then. I really thought I fucked my ESC because of this getting hot thing. The motor spun without me pulling the trigger, but it will work fine if I clean the adapter. :head_bandage: 
I hope your mount will come fast!
```

---
## \#25 Posted by: DaveMess Posted at: 2017-02-16T00:48:08.414Z Reads: 35

```
Oh I understand now. So you just pushed the wires into the connectors? Yeah those have to be soldered. The solder not only holds the wires, but also helps conduct current. You wouldn't be able to pull any current through a non-soldered connection.
```

---
## \#26 Posted by: DaveMess Posted at: 2017-02-16T19:17:26.639Z Reads: 32

```
I still can't get it to work. Getting this ESC running is my last barrier to finishing this board! I'm plugged into CH2, and it won't accept any throttle input and just does the beeping pattern I described at the beginning. What did you change in the software? And how do you have your receiver hooked up? Basically I need everything you have set up to see if anything I'm doing is different. This is so frustrating!
```

---
## \#27 Posted by: DaveMess Posted at: 2017-02-17T07:09:31.056Z Reads: 31

```
I figured it out. My receiver or transmitter is bad. I have a receiver/transmitter for my RC helicopter, hooked it up to that and it ran like a charm. Of course I can't drive around with a giant helicopter TX but at least I figured out what was wrong! Gonna have to order a new receiver and see if I can get it working.
```

---
## \#28 Posted by: Davey Posted at: 2017-02-24T07:42:10.952Z Reads: 35

```
I'm happy for you. I'm sorry for not replying, had some struggles with exams and my motor pulley :frowning: Which Remote do you have? I'm using the Alien Remote and the software you mentioned above. The Heli Firmware didn't work. Most of the Heli ESCs do not have a BEC included, for some reasons. So the Heli Firmware just didn't power my receiver. I plugged the ESC into Ch2 of the receiver, yes. I'll finish my build on this weekend and send you some pics then.
```

---
## \#29 Posted by: DaveMess Posted at: 2017-02-24T11:46:55.893Z Reads: 34

```
It's the alien remote. The receiver is defective and he sent me a new one. Hopefully I'll get it soon, I don't know how long it'll take to reach me.
```

---
## \#30 Posted by: Davey Posted at: 2017-02-24T22:30:42.771Z Reads: 37

```
Has your motor mount arrived yet?
```

---
## \#31 Posted by: DaveMess Posted at: 2017-02-24T22:44:26.570Z Reads: 37

```
<img src="/uploads/db1493/original/3X/d/4/d48e6276e98792f4dacead987bab42e9388d9c7a.jpg" width="690" height="388">Sure did, last week
```

---
## \#32 Posted by: Davey Posted at: 2017-02-25T20:06:03.492Z Reads: 33

```
Oh yeah, this looks awesome
```

---
## \#33 Posted by: DaveMess Posted at: 2017-02-25T20:17:36.853Z Reads: 29

```
Thanks Davey! I'm excited.
```

---
## \#34 Posted by: Davey Posted at: 2017-02-26T10:30:48.106Z Reads: 30

```
I am too! Seems like we'll finish our builds nearly at the same time :smile:
```

---
## \#35 Posted by: Davey Posted at: 2017-03-05T12:26:31.817Z Reads: 29

```
So Dave, how's you build going? I finished mine yesterday, but need to do some changes in the breaking section of the ESC.
Has your second receiver arrived yet?
```

---
## \#36 Posted by: DaveMess Posted at: 2017-03-06T14:08:46.014Z Reads: 26

```
Yes, everything's working normally now. I haven't gotten much chance to ride however since it's been so cold
```

---
## \#37 Posted by: Davey Posted at: 2017-03-06T20:49:55.759Z Reads: 29

```
I had a ride about an hour ago. Need to learn driving again haha... It's not that easy.. I'm happy we finished our builds safely. My ESC also works fine now. 
Where have you put your motor timing degrees? I put mine at 5 and it works fine.
Which acceleration mode have you chosen? I took extra soft throttle acceleration for the moment and it's okay.

I made something like an overkill with using a 430kv motor (on a 6s battery)... Do you know a way to reduce the maximum spinning of the motor via the ESC? Like to set the maximum voltage output?
```

---
## \#38 Posted by: DaveMess Posted at: 2017-03-06T21:30:17.666Z Reads: 30

```
Haha I have to learn this too. It doesn't compare to riding a regular longboard at all! Very different sensation. I have my throttle set to soft, I think the thing that helped me the most was setting the throttle curve to exponential. That means the low end is more gradual than the standard linear curve. Give it a try. 

As far as the motor, you could try messing with the power % but idk if that'll just reduce acceleration or your top speed. You'll have to experiment a bit with that.

For motor timing I have it at 3 which was the stock setting for me. Not sure what that does tbh.
```

---
## \#39 Posted by: Davey Posted at: 2017-03-07T06:24:22.816Z Reads: 32

```
I think I need to try out this exponential thing too. The start power (I think) labels how fast the motor can work. I now have mine at 5 or 10% and the motor powers up slowly. 
So after plugging the batteries the motor needs half a minute to start, but then works fine. So it neither reduces top speed nor acceleration, just the time the motor needs to power up. 

This text explains motor timing degree quite well: https://www.rccaraction.com/its-about-time-how-to-understand-brushless-motor-timing/

That's why we have the timing on a low setting. To get the maximum power on the beginning, so without the motor spinning to much.
```

---
## \#40 Posted by: DaveMess Posted at: 2017-03-08T02:44:41.972Z Reads: 30

```
I see, thanks. I'll be grounded for the next week or so due to cold weather again.. ugh. Winter needs to piss off lol.
```

---
## \#41 Posted by: Davey Posted at: 2017-03-10T17:41:01.621Z Reads: 23

```
Yeah the bad weather really sucks. Do you know a way to reduce the maximum rpm? I overkilled my setup with a 430kv motor and it spins too fast. So is there an option on/in the ESC (program)?
```

---
## \#42 Posted by: DaveMess Posted at: 2017-03-10T18:14:22.528Z Reads: 24

```
I really don't think so. You're going to have to experiment changing things like I said before. Otherwise change your gearing or change your motor are the only things I can suggest.
```

---
## \#43 Posted by: Davey Posted at: 2017-03-11T17:45:54.130Z Reads: 27

```
Okay. So today I had my first real ride and it's amazing! I set the "Start Power" to "Auto" and the Throttle to "very soft" and it works fine. Even tho I only have a single motor setup I cannot say that the one wheel drive is a big deal (in terms of carving because some said that the one wheel drive will push you to the left (if it's mounted on the right)). 
Drive safe!
```

---
## \#44 Posted by: DaveMess Posted at: 2017-03-11T18:19:21.635Z Reads: 25

```
That's awesome, man. I'm also only on one motor right now due to technical issues but Bruno is fixing it for me. I won't be riding anymore for a while but I did get about 6 miles on it with the one motor and it was so much fun. I'm so excited to keep riding but I need to build a real case to protect my investment. The case I have is a very shoddy plastic container lol.
```

---
## \#45 Posted by: Davey Posted at: 2017-03-12T19:04:50.372Z Reads: 26

```
I also have a plastic container, but it's very stable and also has a handle. I screwed it onto my deck and now I can use the handle to carry my board. This helps a lot :wink:
```

---
## \#46 Posted by: Trdolan03 Posted at: 2017-07-11T14:50:46.959Z Reads: 22

```
What firmware did you guys settle on using? Also, you can change the max power (next to the start power) which should limit some of that I think.
```

---
## \#47 Posted by: DaveMess Posted at: 2017-07-11T16:18:57.485Z Reads: 26

```
I am currently using the firmware the ESC comes with originally, I can look at the build number later today if you want me to. Honestly I haven't been riding much at all because my remote/receiver from Alien Power decided to have connectivity issues and dumped me off my board at 20 or so mph.. I had some really nasty roadrash despite my pads and helmet, I'm lucky I wear a helmet or I'd probably have had a massive concussion. So I've been a little gun shy as far as eboarding recently haha. Any other questions about the ESC or whatever else feel free to ask here and I'll try my best to help.
```

---
## \#48 Posted by: Davey Posted at: 2017-07-15T13:51:40.697Z Reads: 29

```
So I changed the start power to 10% since it was very hard for me to get a safe start, but this definitely depends on your motor. And I use the firmware that @DaveMess recommended somewhere above. And I have no connection issues with the remote fortunately. But I have the problem that my board needs like 30-60 seconds to get started. Not that big of a deal, but I think it's weird. But from my experience this has nothing to do with the start power nor with the remote.
```

---
## \#49 Posted by: Trdolan03 Posted at: 2017-07-20T05:40:41.878Z Reads: 29

```
@Davey I had similar problems and re-uploading the firmware seemed to solve it.
```

---
## \#50 Posted by: Trdolan03 Posted at: 2017-08-23T18:06:45.828Z Reads: 19

```
Hey guys I'm back. I'm having an issue with my motors not spinning at all in bench tests and not working with the sensor wires hooked up. Also, I have to keep the "idle" speed to where you have to hold the break for it to stay still or nothing will happen when you try to start the board. Any ideas?
```

---
