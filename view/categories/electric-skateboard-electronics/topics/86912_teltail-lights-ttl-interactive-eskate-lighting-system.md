# TelTail Lights (TTL) - Interactive eSkate Lighting System

### Replies: 92 Views: 3838

## \#1 Posted by: Ricco Posted at: 2019-03-12T01:34:18.229Z Reads: 639

```
Hey guys,

For the past 2 and a half years, I have been working on an interactive lighting system for diy electric longboards.

It all started when I was in college and decided to add head, tail, and RGB side lights to my longboard. I wanted lights that would turn off when I picked the board up and turn on when I dropped it back down, so I created a controller that would take IMU measurements and turn them on and off based on the board’s orientation. Shortly after finishing that project, I started a project based course in which we got to build any embedded systems project we wanted. My team decided that we would build off of my hobby project and make an electric longboard with interactive lighting, a HUD, and various safety systems built in. When that project was completed, I was allowed to keep all of the parts we used since I was the only longboarder in the group :smile: Since I had most of the expensive parts already, I decided to make my own proper electric longboard. When looking into motor controllers, I was immediately sold on the VESC because of it being open source and the awesome, dedicated community it had. When looking further into the VESC I realized that I could integrate my lighting controller project with it to gather motor data and use that to further the lighting effects that I had already created. That’s when I made the first version of what I am now calling the TelTail Lighting System.

My goal when I started this project was to create a lighting controller that was tailored to my system only and didn’t consider making it flexible to meet the needs of other community members. However, as the project matured, I kept adding features that accomplished just that and finally decided that I would go for it.

The first version I made was designed to plug directly into the original VESC.

![TelTail%20v1|500x500](upload://mfoFBK0AwAMJeMJ3G48hG1sGasG.jpeg) 

That worked well for my purposes, but by the time I decided I would share the design with the community, the VESC hardware had changed. So I updated the design to use the same 2mm JST headers used on the VESC for all external connections. This allows the lighting controller to be a plug and play module and provides vibration resistant connections. I also removed the SD card slot and added a 12v buck circuit to the design. I removed the SD card slot because I began developing an android app and was able to log data through that instead.

![TelTail%20v2|500x500](upload://1Ln5C3PW4F9abUuBuOh8J5xgYM2.jpeg) 

After doing some testing with the v2 design, I found the 12v buck circuit I was using to be unreliable. Because of this, I updated the converter to a more dependable one. The new converter is rated for 30W @ 12v, which is just enough to supply power to the head, tail, and side lights. I also removed all unused connector pins to make room for 3 more ports; a 12v output, an auxiliary switched 12v output, and an input for the button channel of a PPM remote.

![TTL%20CM%20SP%20Assembled%20Iso|523x500](upload://5Kf11KNXqR5gNgN4UIWDlbHNllj.jpeg)

To give people options, I also created a second variant of the design that replaces the 12v buck converter with a spring loaded terminal block. This variant is cheaper and allows the user to supply power to the control module using a more powerful DC to DC converter like the one [here](https://www.amazon.com/gp/product/B072PQL72Z/ref=as_li_qf_asin_il_tl?ie=UTF8&tag=solidcircuits-20&creative=9325&linkCode=as2&creativeASIN=B072PQL72Z&linkId=e447cfd5987e48843c705049de0ee7ad). The connector is rated for 10A so you can even supply upwards of 60W withought issue.

![TTL%20CM%20EP%20Assebled%20Iso|642x500](upload://4vUYRLYS36IZDGikYL4VaKXKQ3s.jpeg) 

The auxiliary output was added to v3 of the control module to allow the user to control a 12v motorcycle horn like the one found [here](https://www.amazon.com/gp/product/B01AUYK4EC/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B01AUYK4EC&linkCode=as2&tag=solidcircuits-20&linkId=56deb79ae1ab714bcb11e0b28d7b2938), however, the FET on the TelTail Lights (TTL) control module will get fried if the horn is driven directly from this output. To solve this issue, I designed the High Power Control Module (HPCM). This expansion module allows the aux output to control a FET that is capable of driving the horn without burning up.

![HPCM%202v2%20Assembled%20Iso|562x499](upload://6wiYZEF7fzc9EFV0oW7PoVmGOjP.jpeg) 

When I started developing the TTL control module, I could not find a 12v headlight or tail light that suited my needs so I decided to design my own. For the headlight I wanted something that mounted under my board, was bright enough to light my way on a road or path, and was not glaring in the eyes of people I passed by. To do this, I designed a PCB with 2 bright white LEDs, designed a 3D printable housing that mounts to my trucks like an 1/8" riser, and used oval lenses that cast the light in a wide narrow beam low to the ground.

![Headlight%20Housing%20Front%20Iso|650x500](upload://b1qRfkxNjKQ9amxklAMaGYfLLv2.jpeg) 

For the tail light, I wanted something that created a bright red light but did not cast that light into the eyes of people behind me. To do this, I designed a PCB with 3 bright red LEDs and a housing that mounts to my trucks like an 1/8" riser and diffuses the light to create a glowing bar that lights up the ground around it.

![Tail%20light%20Housing%20Front%20Iso|673x500](upload://3uY6O9IWnmMirHWZBhCA3j3h2Es.jpeg)

I have a couple videos of the lights and their effects on my instagram page, here's the link if you want to check them out: https://www.instagram.com/mattsauve/

Since I have seen many people already use lights like Shredlights, flashlights, or floodlights, I wanted to provide a way to use the TTL control module to control those lights as well. To do this I designed the Low Power Control Module (LPCM). This module allows you to control the power switch of a light with a built in battery using one of the switched outputs of the TTL control module.

![LPCM%201v0%20Assembled%20Iso|636x499](upload://nC8WxqILi4aQJ7qYlga469mhQJg.jpeg) 

The latest module that I designed is the Analog to Digital (A2D) Module. I made this module because I want to be able to control digitally addressable RGB LED strips with the side light ports of the control module. Though I have tested that the functionality of the module works, I haven't developed the code to actually utilize it yet. Once I make all of the firware and app code for this project opensource, I hope that people in the community will help write this portion.

![A2D%201v0%20Assembled%20Iso|690x458](upload://riBcijpdHEGDxOGbwZ5xGAsgqtR.jpeg) 

As mentioned above, I've began developing an app for the TTL System. The app has four main functions. The first is used to configure all of the settings of the TTL control module. The settings include: LED mode characteristics, module orientation, and how the eboard remote controls the lights.

![LED%20Modes%20Static|281x500](upload://ox9x38AoBznFsqALaLKPgw51Fjb.jpeg) 

The second function of the app is to read out live data from the control module. There are 2 screens where live data can be viewed: the motor data screen and the sensor data screen. The motor data screen has a graph at the top that displays whatever information the user selects from below. Below the graph is a list of all the data read from the connected VESC based ESC with checkboxes next to them to select which item are displayed in the graph.

![Motor%20Screen|281x500](upload://kHaoj3al0LimC6oSgPv9Gt46FYJ.png) 

Like the motor data screen, the sensor data screen has a scrolling graph at the top that displays whatever readings you want. The data available is all of the IMU measurements, the calculated board heading, the light sensor reading, and the remote joystick and button states.

![Sensor%20Screen|281x500](upload://qLwd3XbXnuTspxackwNknKqkVbR.png) 

The third function of the app is to track the users path during a given ride and provide stats from that ride. On the map screen, the users rider path is displayed on the map at the top. Stats from the displayed ride are shown below the map. The stats include current longitude/latitude/altitude, currect speed, max speed, and distance travelled. 

![map_edited|281x500](upload://eICmUAFdcIqmc9PVckhvQYLsq0Q.png) 

The fourth function of the app is to provide the user with a backup remote in case their primary remote dies or will not connect. The remote screen uses a relative joystick interface to control the throttle of the VESC based ESC. Wherever the user first places their finger will be the center of the joystick. If they move their finger up, it will increase the throttle. If the they move their finger down, the ESC will start braking.

![Remote%20Screen|281x500](upload://hrkOCRXnGFnE6Gem4Dp1bijQ2aP.png) 

I believe I am finally at the point where I can start selling the various modules that make up the TelTail Lights Project. I have created a website both as a project documentation location and a webstore for purchasing the boards that I've designed. I do not have anything in stock yet, though, because I wanted to gage everyone's interest on this forum before having boards assembled. Please take a look at the links below to read more about the project, browse the items I want to sell, and download related files. Please keep in mind the prices in the store are all estimates at the moment. They will be updated once I gage interest and order assembled modules.

**_TLDR_**: [u]System Overview[/u] (for more detailed info visit the documetation page of my site)

[details="TTL Control Module Features"]
* 9 switched 12v DC outputs 
  * Head light
  * Tail light
  * Side RGB lights (6 total outputs)
  * Aux output (designed to control a horn)
  * 2A max each
* VESC communication (currently I2C, planned to change to UART)
* PPM button input
* Nunchuck port (a pass through of the VESC comms)
* Direct 12v DC output (for use with HPCM or other external devices)
* Light Sensor Input (to be implemented in code)
* BLE to connect to Android app
* Two Types
  [details="Self Powered (SP)"]
  * Input Voltage: 20 – 50v
  * Max Power Output: 30W (includes control logic)
  * Power Connector: Male XT30
  [/details]
  [details="Externally Powered (EP)"]
  * Input Voltage: 12v @ 10A max
  * Max Power Output: Determined by DC converter used
  * Power Connector: 16-24 AWG Screwless Terminal Block
  [/details]
[/details]
[spoiler][/spoiler]
[details="Low Power Control Module Features (LPCM)"]
* Plugs into a switched output of the TTL Control Module
* Used to control battery powered lights
  * Flash lights
  * Flood lights
  * Shred Lights (not yet tested)
  * Controlled Voltage: 30v max
  * Controlled Current: 3A max
[/details]
[spoiler][/spoiler]
[details="High Power Control Module Features (HPCM)"]
* Plugs into a switched output of the TTL Control Module
* Used to control horns or high current devices
  * [Flood lights](https://www.amazon.com/Willpower-Square-Driving-Off-Road-12V-24V/dp/B01M7Y382H/ref=sr_1_4?crid=1SVYL62RHU0A9&keywords=48w+led+light&qid=1552963111&s=automotive&sprefix=48w+%2Cautomotive%2C161&sr=1-4)
  * [Horns](https://www.amazon.com/gp/product/B01AUYK4EC/ref=as_li_tl?ie=UTF8&camp=1789&creative=9325&creativeASIN=B01AUYK4EC&linkCode=as2&tag=solidcircuits-20&linkId=56deb79ae1ab714bcb11e0b28d7b2938)
  * Controlled Voltage: 60v max
  * Controlled Current: 30A max
  * Flyback diode included for horns (deconfigurable through PCB jumper)
[/details]
[spoiler][/spoiler]
[details="Analog to Digial (A2D) Module Features"]
* Connects to a side light port of the TTL Control Module
* Designed to control digitally addressable LED strips
* **Not yet implemented in the code** 
[/details]
[spoiler][/spoiler]
[details="Android App Features"]
* Configure the lighting effects of the TTL system
  * Sensored control can be turn on/off (turns lights off when the board is picked up)
  * Light control can be turned on/off (not yet implemented)
  * 9 modes for side RGB lights
    * Static - Set each side light to a solid color you choose
    * Color Cycling - Cycles through all colors at the rate and brightness you choose
    * Compass Cycle - Controls the color based on the orientation of the eboard
    * Throttle Based - Control the color based on the throttle position
    * RPM Based - Controls the brightness based on RPM and the color cycles
    * RPM + Throttle - Controls the brightness based on RPM and color based on throttle
    * X Accel Based - Controls the brightness based on the x-axis accel reading 
    * Y Accel Based - Contols the color based on the y-axis accel reading 
    * Custom - choose for the various brightness and color bases to create your own effect
* View live data from connected VESC in text and on a scrolling graph
* View live data from the on-board IMU in text and on a scrolling graph
* View ride path and stats
* Control the motor's throttle with virtual remote (meant as a backup remote)
* Get notified of fault codes issued by the VESC
* Log data gathered from the VESC, IMU, and/or GPS
* Configure how your remote controls the TTL system
  * PPM and Nunchuck supported (UART remotes are planned to be added)
  * Enable or disable turn signals (currently only working with Nunchuck) 
  * Customize the output type of the aux output
    * Toggled
    * Momentary
    * Timed
    * Pattern (not yet implemented)
  * Customize what button presses perform specific actions
    * Actions:
      * Aux Control
      * Toggle All LEDs
      * Toggle Headlights
      * Toggle Side Lights
      * LED Mode Up
      * LED Mode Down
    * Button press types:
      * Single Tap
      * Double Tap
      * Triple Tap
      * Hold > 0.5s
* Calibrate the IMU
* Set the oriantation of the TTL Control Module
  * Allows you to place the control module however you like in your build
[/details]


Since this project has been my hobby project for a long time now, I have decided I have taken it as far as I want on my own, and I will be making it open sorce. That way anyone interested can help further the developement and new features can be rolled-out regulaly. I have posted the schematics and files required to assemble all of the boards to the downloads page of my website (link below). I have also created git repos for both the firmware and and the android app (links below). The only thing I will not be releasing as open source is the PCB designs. I have put countless hours of work into the PCB designs alone so I will be selling them on my site but not releasing the designs. 

The app can be found on the Google Play Store [HERE](https://play.google.com/store/apps/details?id=com.solid.circuits.TelTail) 

Please visit my site to learn more about this project
* Documentation: https://solidcircuits.net/documentation/
* Downloads: https://solidcircuits.net/downloads/
* Store: https://solidcircuits.net/shop/

The code for the TTL control  module firmware can be found [HERE](https://github.com/Samatthe/TTL-Firmware)

The code for the Android app can be found [HERE](https://github.com/Samatthe/TTL-App)

I have pictures and videos of my project posted on my instagram page, here's the link if you want to check them out: https://www.instagram.com/mattsauve/
```

---
## \#2 Posted by: venom121212 Posted at: 2019-03-12T01:40:26.054Z Reads: 495

```
This is a really great project man! I'm definitely keeping an eye on this. Truly great work
```

---
## \#3 Posted by: sofu Posted at: 2019-03-12T01:55:13.459Z Reads: 481

```
Wow, this is really cool work! Awesome job!
```

---
## \#4 Posted by: mishrasubhransu Posted at: 2019-03-12T01:56:18.339Z Reads: 475

```
This is awesome. It could become the open source metr pro(the app side of things) as more contributors put their time in this.
```

---
## \#5 Posted by: maxpriority Posted at: 2019-03-12T03:26:28.013Z Reads: 448

```
Sweet, I'm looking forward to seeing how this progresses.

While I appreciate the flexibility, I don't want to spend too much time on solutions for my board, so I'd be sold a kit where everything is included.
```

---
## \#6 Posted by: Ricco Posted at: 2019-03-12T15:09:03.525Z Reads: 414

```
@venom121212 @sofu Thanks for your support! :blush: 

@mishrasubhransu I really hope so. I have A LOT of ideas for what to do with the app and control module but very little time to implement them, so help from the community would be awesome!

@maxpriority I was originally thinking I would sell whole kits, but what's holding me back is all of the 3D printed parts and the cables. I only have one 3D printer and the headlight base alone takes somewhere around 4 hours to print. I could print multiple at once but it's still more of a hassle than I would like. The cables are easy to provide when they are short (i.e. to ESC, to PPM receiver, to an expansion module), but I have not found an easy way to make the long cables. I cannot find a supplier for long pre-crimped wires, and if I order custom cables they become prohibitively expensive :frowning:
```

---
## \#7 Posted by: moon Posted at: 2019-03-12T15:12:59.717Z Reads: 376

```
[quote="Ricco, post:6, topic:86912"]
but I have not found an easy way to make the long cables. I cannot find a supplier for long pre-crimped wires, and if I order custom cables they become prohibitively expensive :frowning:
[/quote]

@Andy87

maybe you can help?
```

---
## \#8 Posted by: venom121212 Posted at: 2019-03-12T15:16:35.547Z Reads: 358

```
I just bought my second 3d printer. I can assist if necessary!
https://giphy.com/gifs/photoset-adventure-time-advice-uEfiRQmK4jzJC
```

---
## \#9 Posted by: Andy87 Posted at: 2019-03-12T16:26:40.399Z Reads: 344

```
I‘m not through everything, but which wire in which length you need @Ricco
```

---
## \#10 Posted by: Kingdom421 Posted at: 2019-03-12T16:30:32.312Z Reads: 334

```
Groundbreaking innovations is why I love this community.
```

---
## \#11 Posted by: Ricco Posted at: 2019-03-12T16:49:33.208Z Reads: 329

```
Thats great, having someone helping with the printing would definitely make the kits more feasible :smile:
```

---
## \#12 Posted by: Dornacht Posted at: 2019-03-12T16:50:22.317Z Reads: 325

```
@Ricco so are the rear lights controlled by a filtered accelerator or sensing from the vesc?
```

---
## \#13 Posted by: Ricco Posted at: 2019-03-12T17:05:02.281Z Reads: 332

```
I am using 24AWG for all of my cables. There are 4 cable types that I need to source:

* Headlight: 26in., 2pos, female to female 
* Tail Light: 16in., 2pos, female to female
* Side Lights: 13.5in., 4pos, female to wire
* Horn: 23in., 2pos, female to wire

These are the lengths I am using in my board. The wire lengths needed would vary from project to project based on where the control module is located and how they are routed, but we may be able to work lengths that suit the majority of use cases.
```

---
## \#14 Posted by: Ricco Posted at: 2019-03-12T17:09:25.534Z Reads: 319

```
The rear lights are controlled based on the throttle position read from the VESC. The brightness ranges from 50% when not breaking, to 100% when at full brake.
```

---
## \#15 Posted by: butt_stallion Posted at: 2019-03-12T17:11:03.222Z Reads: 323

```
![shutupandtakemymoney|500x313](upload://1AFVnPPMni3Pjj8XzgJ6qyt3Fpj.gif)
```

---
## \#16 Posted by: Mich21050 Posted at: 2019-03-12T17:13:03.266Z Reads: 311

```
This whole thing is awesome... Way better than mine.. :slight_smile:

Any plans on making the code open source? :slight_smile: 

(Btw:: Check your links...downloads) :slight_smile:
```

---
## \#17 Posted by: butt_stallion Posted at: 2019-03-12T17:16:21.353Z Reads: 300

```
Using your control module, would it work if I ran my own LEDs ?
```

---
## \#19 Posted by: Ricco Posted at: 2019-03-12T17:23:48.841Z Reads: 310

```
Thank you :) Your project is great too. Now there are two options for open source lighting controllers at different price ranges :smiley: 

I do plan to make the code open source. I just need to get put the right licensing on it and make some git repos.

Thanks for pointing out the link. Its fixed now.
```

---
## \#20 Posted by: Ricco Posted at: 2019-03-12T17:30:55.915Z Reads: 314

```
In short, yes. The control module switches 12v on all of its LED ports. As long as your LEDs operate off of 12v and draw less current than what will damage the FETs or power supply, they can be controlled. Take a look at the [documentation page](https://solidcircuits.net/documentation/) of my site to learn more about the current capabilities of the control module.
```

---
## \#21 Posted by: Andy87 Posted at: 2019-03-12T19:52:31.171Z Reads: 305

```
Which size plugs you use? 2mm jst or 2,5mm jst and how much cables you think you will need from each?
It’s not a big thing to just crimp the cables but it takes some time and the wires would need to be ordered as well.
```

---
## \#22 Posted by: Ricco Posted at: 2019-03-12T21:25:33.862Z Reads: 279

```
They are all 2mm JST PH connectors. Ya the time spent on crimping is the part that I am trying to avoid since there would be about 18 crimps to perform per kit. Thats counting 1 headlight cable, 1 tail light cable, 2 sidelight cables, and 1 horn cable. The ESC adapter cable and the PPM reciever adapter can be made with pre-crimped wires bought from digi-key.
```

---
## \#23 Posted by: Ricco Posted at: 2019-03-13T20:53:52.361Z Reads: 265

```
https://www.instagram.com/p/BZuKVibnuy1/?utm_source=ig_share_sheet&igshid=ssimk4b7mu4e
Here's a demo of the control module's Auto-On/Off feature. It uses the on board IMU to sense when the board is kicked up or picked up and turns off the lights. When the board is dropped back down, it turns the lights back on.
```

---
## \#24 Posted by: Ricco Posted at: 2019-03-14T00:51:55.785Z Reads: 262

```
https://www.instagram.com/p/BbvvnwtHbQ7/?utm_source=ig_share_sheet&igshid=o96kcsyyvdh1

Here's a demo of the "Compass Cycle"  lighting effect. It uses the gyro measurement to keep track of what direction the board is pointing and uses that to set the color of the lights. It cycles through all colors every 180 degrees that the board is turned.

These two demos are the only ones that I have at the moment. I plan to post more soon, but my priority at the moment is to get the code posted.
```

---
## \#25 Posted by: Ricco Posted at: 2019-03-16T22:07:55.445Z Reads: 238

```
I just posted the firmware and app code to github, so now the project is officially open source :grin:

The firmware can be found [HERE](https://github.com/Samatthe/TTL-Firmware)

The Android app can be found [HERE](https://github.com/Samatthe/TTL-App)

Now that the code is up, I want to have some people be beta testers. Since I've only tested the system with my board, I want to ensure it will work for everyone before making them available to all. If you would like to be a beta tester please DM me so we can set something up :slightly_smiling_face:
```

---
## \#26 Posted by: butt_stallion Posted at: 2019-03-17T20:47:43.278Z Reads: 226

```
PM'ed about beta testing
```

---
## \#27 Posted by: linsus Posted at: 2019-03-17T21:13:00.650Z Reads: 231

```
good work! following! would be nice with a small features list to see what it actually does/what is implemented. Something like;

brake lights

head lights on/off

color shifting based on orentation

etc.
```

---
## \#28 Posted by: Sn4pz Posted at: 2019-03-17T21:23:10.533Z Reads: 222

```
Sorry if this has already been touched upon, but Is there a version in the works for Trampa builds? :slight_smile:

My late night rides would benefit greatly by having a dependable light system 😂😂
```

---
## \#29 Posted by: Ricco Posted at: 2019-03-18T04:09:17.067Z Reads: 215

```
@linsus Thank you :slight_smile: As you suggested, I will add a feature list to the topic post soon. I didnt add one to begin with because I didnt want the post to become too long :stuck_out_tongue:

@Sn4pz Typically the trampa builds I've seen use high powered flood lights like the one [here](https://www.amazon.com/Auxbeam-Waterproof-Motorcycle-Mounting-Brackets/dp/B00T7L0DKK/ref=sr_1_7?keywords=36w+led+bar+%3Blight&qid=1552881562&s=automotive&sr=1-7). Using the externally powered control module, the HPCM, and an appropriately rated 12v DC converter, one of these lights could be controlled. I have not designed any case for my lights that would mount to a MB but I hope someone in the community will do so in the future :slight_smile:
```

---
## \#30 Posted by: Sn4pz Posted at: 2019-03-18T04:11:44.831Z Reads: 214

```
Thanks for the link! Unfortunately my Trampa wont be a hardcore offroader, so im going for more of a sleek and slick build :) 

Hopefully someone makes that soon :rofl: Ive not the idea slightest how to
```

---
## \#31 Posted by: Ricco Posted at: 2019-03-18T14:04:30.353Z Reads: 207

```
No problem! If you want something more sleek then a light like [this one](https://www.amazon.com/dp/B00NPQUYM0/ref=twister_B00NPQUX3A?_encoding=UTF8&psc=1) might be a better option. You would still need to find a way to mount it, but this kind would be pretty easy to mount to your trucks.without 3D modeling/printing.

I also suggest scrolling through the [eSkate Lights Thread](https://www.electric-skateboard.builders/t/eskate-lights-thread/199) to see if there are any lights on there you like. Someone may have already done exactly what your looking for :slight_smile:
```

---
## \#32 Posted by: Ricco Posted at: 2019-03-19T03:25:14.705Z Reads: 202

```
I've added a "System Overview" section with a list of features for each module and the Android app to the bottom of the topic post. Check it out to get a better understanting of what the system can do :slight_smile:
```

---
## \#33 Posted by: bsancken Posted at: 2019-03-19T06:37:09.981Z Reads: 211

```
Trampa build here! Definitely like the headlight/ RGB/Addressable led options! 

Another module (since you seem to have the resources) that I would pay a significant amount for is a UART multiplexer/ splitter so we can connect more than one thing. Personally, I would like to connect a lighting controller, BMS, Bluetooth module, and possible a smart remote to this but only have 2 ports on my dual FocBox build. Not sure if something like this is possible or not. 

I love this whole thing though!
```

---
## \#34 Posted by: linsus Posted at: 2019-03-19T11:52:49.819Z Reads: 207

```
Skimmed thru some of the documentation and saw that you use the Nyko Kama,(I use the same but with NRF mod) 

I have one implementation on the wishlist for any nunchuck based controller: Ability to toggle turnsignals with Left/Right on the nun-chuck. Could be separate LEDs or trigger the left/right leds on underside of board to flash yellow f.e. 

Turn signals could be turned off by pushing the direction again or just set with a timer.

Thoughts?
```

---
## \#35 Posted by: Ricco Posted at: 2019-03-19T14:25:27.080Z Reads: 213

```
@bsancken Thanks for your support! I agree a UART multiplexer would be a great addition. The problem with just splitting the UART signal to all the devices is that the communication is asynchronous so the devices will keep trying to talk over each other and end up corrupting the data. I wish I2C was the standard for communicating with VESCs since it allows for a large number of devices to be connected to a single bus and each has its own address. But that wouldn't work for the Bluetooth modules people use for connecting to phone apps so there are trade offs.

I will definitely look further into making a UART multiplexer. I am thinking a SAMD21 that is programmed to act as the middle man between the VESC and the other UART devices would do the job. The SAMD21 has 6 SERCOM ports that can all be configured to UART, so theoretically up to 5 devices would be able to be supported :stuck_out_tongue:

@linsus I actually do have turn signals implemented for Nunchuck remotes, I just forgot to add it to the features summary. It's been added now :P The way my implementation works, is that to activate the left/right turn signal the user needs to push the joystick to the left/right while holding the Z button down. The turn signals will be active for as long as the user holds the joystick left/right and the button down.
```

---
## \#36 Posted by: linsus Posted at: 2019-03-19T15:25:00.135Z Reads: 188

```
Z button, thats change motor direction for me. sounds scary :laughing:
```

---
## \#37 Posted by: Ricco Posted at: 2019-03-19T16:47:28.139Z Reads: 187

```
Haha Sorry I miss spoke. It is the C button that I use for control with the nunchuck. Z button would still work for changing the motor direction or cruise control :sweat_smile:
```

---
## \#40 Posted by: Sn4pz Posted at: 2019-03-21T01:34:01.542Z Reads: 188

```
you should pm the seller instead of using their thread
```

---
## \#41 Posted by: CharlieFlan Posted at: 2019-03-21T02:15:56.841Z Reads: 190

```
Don’t suppose this works on any prebuilt boards eh?
```

---
## \#42 Posted by: Ricco Posted at: 2019-03-21T02:27:37.793Z Reads: 215

```
What kind of pre-built boards are we talking? There are a few things to consider:

1. Is there enough space inside the enclosure for the control module + wires?
2. Is the ESC a VESC based ESC? If not then the lighting effects that are based on info from the ESC will not work (i.e. RPM or throttle)
3. What kind of remote does it use? If it is a PPM remote that has a button channel and you can access the receiver, you can control the lights whether the ESC is VESC based or not.

Even if the ESC is not a VESC based ESC and the remote is not a PPM remote, you could still make use of the lights as long as there is room inside the enclosure or the control module + wires. You would then be limited to controlling the lights through the app, but would still be able to use all of the lighting effects that dont rely on info from the ESC.
```

---
## \#43 Posted by: CharlieFlan Posted at: 2019-03-21T03:00:37.740Z Reads: 204

```
Interesting. Will be in touch with you later!
```

---
## \#44 Posted by: SmokeyRider Posted at: 2019-03-23T20:19:45.677Z Reads: 190

```
@Ricco Are we talking neopixels here? or just plain rgb strips?

double respect if you went with neopixels
```

---
## \#45 Posted by: Ricco Posted at: 2019-03-23T21:02:23.691Z Reads: 183

```
The controller is designed to control analog RGB led strips by default. The A2D Module shown in the original post was created to give the controller the ability to control all types of addressable LED strips including neopixels. Unfortunately, the code for utilizing the A2D Module hasn't been implemented yet but is planned to be in the future.
```

---
## \#46 Posted by: Ricco Posted at: 2019-03-25T17:49:15.739Z Reads: 184

```
I am still looking for **beta testers**.

Dont worry about skill level or resources. If you are interested in hooking the system up to your board and giving me feedback to improve it, just send me a message. If you tell me about your build, I will work with you to find the best way to make my system work   :slight_smile:
```

---
## \#47 Posted by: Bobby Posted at: 2019-04-27T16:37:46.306Z Reads: 172

```
I love this system! Few problems occur with trying to map onto the remote but using the app on the phone wirks great.... haven’t been able to get anything besides color cycle and color compass....the head lights arent as bright as i had hoped. They are more for being seen than 
to see obstacles in your path.
```

---
## \#48 Posted by: RedBaron Posted at: 2019-04-27T16:57:25.546Z Reads: 170

```
I really like the idea of this. Was really considering a purchase,  But it's a little steep in price for the quality of lights. I'd really only be interested in the pcb part and add my own lights.

Edit: I also don't care for the horn. But overall great job in putting it together. Nothing but respect.
```

---
## \#49 Posted by: kuphjr Posted at: 2019-04-27T17:06:55.278Z Reads: 158

```
PMed! This looks like an awesome project. Makes me excited to see what this community has inspired people to do.
```

---
## \#50 Posted by: Ricco Posted at: 2019-04-27T18:30:20.572Z Reads: 164

```
@Bobby I'm really glad you are liking it! With the FW updates I'm making now, you will be able to use the other LED modes that rely on info from the ESC. Ya the lights that I made are bright but not super bright. Having them housed in a 3D printed case without a heatsink makes it difficult to up the brightness since brigter ligths would take more power, causing more heat which would start melting the plastic when when left on for a long time :stuck_out_tongue:

@RedBaron Thank you for your support :slight_smile:  I definitely get the need for brighter, higher quality headlights than the ones I made myself. Thats why I designed the system with the use of other lights in mind :wink: You have a few options to do that. If they are 12v (depending on the current draw) you could connect them directly to the control module. If they have their own battery and power switch you can use the LPCM to control them. If they are high current lights like flood lights and powered from the battey, you can use the HPCM to control them.

@kuphjr Thanks, I agree, it really is cool to see all the different projects that have sprouted up on this forum!
```

---
## \#51 Posted by: RedBaron Posted at: 2019-04-27T18:37:49.672Z Reads: 153

```
Thanks for the explanation. Totally didn't realize you had so many options. I would be interested in a unit  without the extras. And a lpcm for a self powered headlight. I have a 3d printer so I can make my own housing and share the stl as well. I'll check out your site.

Im putting together a new build so im sourcing parts at this time.
```

---
## \#52 Posted by: Ricco Posted at: 2019-04-27T18:53:11.901Z Reads: 158

```
No worries. There is alot to digest relating to this project and all of the features/options might not be easy to understand on first read (or might not be clearly explained :stuck_out_tongue:). There is a ton more information on the [documetation page](https://solidcircuits.net/documentation/) of my site so please do check that out. And please send me a PM if you are interested in getting parts for your new build and helping with beta testing. Having someone test the system with their own lights would be very helpful :slight_smile:
```

---
## \#53 Posted by: Ricco Posted at: 2019-04-27T21:01:03.789Z Reads: 165

```
@Bobby, @venom121212, @butt_stallion, @colinphotovideo, If you guys take any photos or videos during testing, please post them here so that others can see our progress and get an idea of how the system looks / functions.
```

---
## \#54 Posted by: venom121212 Posted at: 2019-04-27T22:04:18.090Z Reads: 164

```
I ran into an issue with my second unity so I can only bench test without disassembling all my waterproofing on my main board :cry:

I have it laid out in my second build with a blank space just waiting for the unity to arrive and get ride footage!
```

---
## \#55 Posted by: Bobby Posted at: 2019-04-28T00:14:08.560Z Reads: 183

```
![image|375x500](upload://9bepMdvgGh3Zlqb6k5Mr1q7PYSq.jpeg) ![20190422_004138|374x499](upload://A5YoC9YnDgPFPpIFZwgCR2Wrycm.jpeg) ![image|500x500](upload://uncAMWSMreO67RoJh5lyV3KhBUk.jpeg) 
https://youtu.be/xEGSKoHqCQ0


A couple of pics and a video of me going around the block with compass mode
```

---
## \#56 Posted by: mynamesmatt Posted at: 2019-04-28T00:34:24.229Z Reads: 175

```
I'll beta test one!
```

---
## \#57 Posted by: Bobby Posted at: 2019-04-28T00:50:38.674Z Reads: 172

```
Im actually planning on getting a second set.... i love it even with everything not working! I can only imagine how great it will be when the firmware gets updated and the bugs get ironed out.
```

---
## \#58 Posted by: Ricco Posted at: 2019-05-03T03:52:05.693Z Reads: 168

```
I finished implementing some pretty major updates last night to the control module FW and the Android App. The most important change is that the control module is now able to communicate with the ESC over UART, so all features of the lighting system can be utilized without changing the FW of the ESC.

The second important change is the addition of a settings menu for the remote. That menu allows you to configure which type of remote you are using and what type of input you would like to use to control the lights. This allows more remotes to control the lights than just ones with a button mapped to channel 2 of the reciever.

@venom121212, The bright side is that now, you can test all features using UART comms right when you get your second Unity :stuck_out_tongue:

@Bobby, Thanks for the pics and video. I'm super happy that you like the system so much without getting to test all the features yet :blush:

@mynamesmatt, Please PM me so we can get the ball rolling.
```

---
## \#59 Posted by: venom121212 Posted at: 2019-05-03T10:54:48.076Z Reads: 165

```
[quote="Ricco, post:58, topic:86912"]
The bright side
[/quote]

I see what you did there :smirk:

Awesome! Thank you for all the hard work
```

---
## \#60 Posted by: Pavlo_H Posted at: 2019-05-20T23:13:50.584Z Reads: 155

```
Is beta testing still going on?
```

---
## \#61 Posted by: Ricco Posted at: 2019-05-21T12:53:00.403Z Reads: 153

```
Ya beta testing is still in progress and is open to for people to join if they want.

I've had a lot of people reach out to me interested in becoming beta testers but only 4 people have followed through with it.

Last week I finished implementing the UART comms on the control module so that no one has to touch the FW of their ESC to get the lights working. At this point, no beta testers have updated the FW of their control modules (life has a way of getting in the way of these things :stuck_out_tongue:) so I am waiting to here back on any bugs with that. There is one known bug that I am currently working on in the meantime as well as some updates I want to make to the tail light control so the down time is not being wasted :stuck_out_tongue:
```

---
## \#62 Posted by: briman05 Posted at: 2019-05-21T13:16:21.068Z Reads: 146

```
i would be down to test but don't have an Android to download the app.  And have a Mac as my main computer
```

---
## \#63 Posted by: Ricco Posted at: 2019-05-22T03:26:54.297Z Reads: 139

```
Ya sorry man, I don't have any iOS devices for developing an app or a Mac to test out the FW updater tool. I hope I can support Apple devices eventually.
```

---
## \#64 Posted by: Bobby Posted at: 2019-05-22T04:56:51.337Z Reads: 135

```
You can buy a cheap android device for 20-40 bux on offer up. Thats what i ended up doing...
```

---
## \#65 Posted by: RedBaron Posted at: 2019-05-22T05:12:50.791Z Reads: 134

```
I'll volunteer to test it for you if you still need people. My deck should be in next week and my build finished by the weekend. I'm pretty diligent with stuff like this so let me know.
```

---
## \#66 Posted by: yelnats8j Posted at: 2019-05-22T13:40:34.914Z Reads: 134

```
[quote="Bobby, post:64, topic:86912"]
cheap stolen android device for 20-40 bux on offer up
[/quote]

Fixed it 

10 char
```

---
## \#67 Posted by: Bobby Posted at: 2019-05-22T14:05:13.666Z Reads: 135

```
Not everything is stolen guy... ever hear of an Obama phone?
```

---
## \#68 Posted by: ZachTetra Posted at: 2019-05-22T14:05:17.431Z Reads: 135

```
What would it take to become a tester?  I'm gonna have a Unity builld running in a month or so and I have a cheap Android I use to program it, located in the US
```

---
## \#69 Posted by: Ricco Posted at: 2019-05-23T15:54:41.845Z Reads: 146

```
@RedBaron, Cool, PM me so we can get it going :slight_smile:

@ZachTetra, To become a beta tester you need to:

1. Be willing to pay for the cost of parts.
2. Be able to communicate clearly
3. Have a windows pc available since this is the only OS the FW updater has been tested on yet. (though Mac or Linux programming should be possible)
3. Be willing to update the firmware from time to time
3. Let me know of any unexpected behavior you experience
4. Give me constructive criticism regarding any aspect of the system that could be improved

Some limiting factors that prevented a few people from becoming beta testers in the parts are:
* Control from the remote required a remote with a button. This is **fixed** with some additional control options
* Features that are based on info from the ESC required the ESC's FW to be changed. This is **fixed** with the implementation of UART comms between the control module and ESC.
* Cost of shipping outside of the US is ridiculous. The lowest price I could find from a trusted shipper is $36 :disappointed: 

Some considerations when thinking of becoming a beta tester:
* The head and tail lights I designed are designed around Caliber II trucks. They will work with a wide variety of trucks but not all. If they dont fit, we can work together to alter the design to work.
* A remote with a button mapped to the recievers second channel is best for controlling the lights. If you dont have a button on your remote and want to control the lights outside of the phone app, you will need to add momentary switch to your enclosure, or use the throttle down/up control method. The throttle down/up control method allows the control module to acknowledge a small flick of the throttle down/up as a button press.
```

---
## \#70 Posted by: RedBaron Posted at: 2019-05-23T16:29:42.703Z Reads: 133

```
Will do, everything sounds pretty reasonable.
```

---
## \#71 Posted by: ZachTetra Posted at: 2019-05-23T17:36:38.168Z Reads: 125

```
I’ve got Paris trucks so it won’t be a perfect fit, but I can add bracketing no problem.  What kind of cost are we looking at for parts?
```

---
## \#72 Posted by: briman05 Posted at: 2019-05-23T17:42:28.610Z Reads: 128

```
I got calibers but my main computer is a Mac but do have a windows computer at work.  but I have the r-spec controller
```

---
## \#73 Posted by: Ricco Posted at: 2019-05-24T02:25:45.759Z Reads: 123

```
I found a programming tool today that works with the bootloader I use and has installations for Windows, Mac, and Linux :smile: I just tested the 64-bit windows version on my computer and everything worked great. This should make programming using a Mac possible.

What do you mean by the "r-spec controller"? Is that enertions nano-x?
```

---
## \#74 Posted by: briman05 Posted at: 2019-05-24T03:20:22.413Z Reads: 121

```
Yeah I couldn’t remember what it was actually called lol? Since it doesn’t really have any buttons I don’t think it would work would it.
```

---
## \#75 Posted by: Ricco Posted at: 2019-05-24T03:37:27.801Z Reads: 130

```
Ok ya in that case it is still able to be used to control the lights. You would just need to use the throttle up/down control mode. I just recently added that setting to support remotes without a button like the nano-x.

In that mode you can flick (or move quickly) the throttle up or down slightly to control the lights. It only has to be a little bit of movement so if you flick it down, you really shouldnt notice the slight amount of braking that is applied as a result. (that is if your ESC is setup for a smooth response in the first place :stuck_out_tongue:) The other option is to add a momentary button to your enclosure an plug it into the button port, but thats not exactly as convienient as controlling the system with your remote.
```

---
## \#76 Posted by: briman05 Posted at: 2019-05-24T03:54:14.627Z Reads: 122

```
I’ll have reread this thread as I skimmed it but I really do like the lights under the board as it would make it easier to be seen at night
```

---
## \#77 Posted by: Ricco Posted at: 2019-05-24T14:40:59.879Z Reads: 133

```
Sorry for skipping over your question. I just PM'd you with further details.
```

---
## \#78 Posted by: Spacecase418 Posted at: 2019-06-05T23:19:45.384Z Reads: 131

```
Night rides are my favorite thing. I have bike lights and underglow created by led attached to a portable cellphone charger. I found this thread looking for horn solutions. How can I become part of the beta group?![image|375x500](upload://rGHHk0qWtod7vEbptOftya6wF1x.jpeg)
```

---
## \#79 Posted by: Saturn_Corp Posted at: 2019-06-06T23:48:48.176Z Reads: 126

```
How bright is that light you have on the front? I need to find another option other than amazon automotive lights with weak mounting systems that snap in half after a week or 2.
```

---
## \#80 Posted by: Sn4pz Posted at: 2019-06-07T00:13:15.548Z Reads: 127

```
Do the lights have a good mounting system(on the light itself)? Is it just the materials of the mounting bracket that are weak?

If yes to both, why not try and make a metal / aluminum / steel version yourself? Even if its not visually appealing, you can always work on it once its functional :P


*ahem* I want a capable / study mount for trampa trucks too...  maybe we can split the cost of RnD and production? :<asd>P *ahem*
```

---
## \#81 Posted by: Saturn_Corp Posted at: 2019-06-07T00:26:41.686Z Reads: 131

```
Yah the lights themselves are great, but it's the brackets that suck. Cheap cast China metal.

![IMG_20190511_115241|690x388](upload://pArVvjzjxTT9yA37dwp2OufBjjN.jpeg) 

![IMG_20190606_172612|281x500](upload://gdsgUJQwdJUSv13T9ARzvB392FB.jpeg)
```

---
## \#82 Posted by: Spacecase418 Posted at: 2019-06-09T05:20:53.573Z Reads: 117

```
It’s a bike light right now 3500lm. I also use a shoulder mounted spelunking light.
```

---
## \#83 Posted by: briman05 Posted at: 2019-06-10T01:42:15.705Z Reads: 111

```
I got mini flashlights and use P clamps with rubber on them to stabilize them.
```

---
## \#84 Posted by: Ricco Posted at: 2019-06-16T06:56:58.574Z Reads: 104

```
Based on feedback from the beta testers, I recently upgraded the LEDs used for the headlights. With these new LEDs the light output increased from ~50lm to ~150lm. The difference is night and day :laughing:

![Areal%20TTL%20LED%20upgrade|690x451](upload://lCUOJZ5G8Mr4cLXsw7AxKaxjZ8w.jpeg)
```

---
## \#85 Posted by: Ricco Posted at: 2019-07-15T18:37:48.357Z Reads: 96

```
Here's a short video of a night ride demoing the TTL system. Please pardon the quality as this was my first time ever using my GoPro to make a ride video :stuck_out_tongue: 

https://www.youtube.com/watch?v=k5TAy0DaudE
```

---
## \#86 Posted by: Ricco Posted at: 2019-08-29T05:42:26.542Z Reads: 84

```
Update: I've added support for GT2B remotes. The TTL system now supports 7 different input control methods:

* Momentary (high when pressed, low when unpressed): TB Nano
* Latched (state toggles with every button press): ?
* Latched PWM (a pwm signal that toggles pulse width with every button press): GT2B
* UART [Chuck Struct] C (UART remote mapping its button to C of the VESC chuck struct): Feather
* UART [Chuck Struct] Z (UART remote mapping its button to Z of the VESC chuck struct): Feather
* Throttle Up (gently tap the throttle forward): Any PPM (PWM) remote
* Throttle Down (gently tap the throttle backwards): Any PPM (PWM) remote

https://www.instagram.com/p/B1u0A2_h1-m/?utm_source=ig_web_copy_link
```

---
## \#87 Posted by: Ricco Posted at: 2019-09-11T18:00:22.234Z Reads: 77

```
Here's a video of me testing the "X-Accel Mode" of the TTL system. This mode takes the X axis accelerometer readings and tries to determine which way you are carving and how hard. The lights on the outer edge of the carve light up and the harder you carve, the brighter they get :smiley: 

https://youtu.be/QfpFpptMPPQ

This mode can definitely use some tweaking, but this proof-of-concept implementation looks pretty promising :smile:
```

---
## \#88 Posted by: annihil8ted Posted at: 2019-10-01T21:34:38.553Z Reads: 66

```
@Ricco, do you still need testers? I'd love to help out! My background is in EECS/Computer Engineering and at the very least, I'm able to provide consistent feedback as I commute daily on my board. This looks very promising!
```

---
## \#89 Posted by: Ricco Posted at: 2019-10-02T06:51:17.638Z Reads: 63

```
Thanks for the support! I do not need more testers at this moment, but once I recieve v4.0 of the HW I will probably need a few more people to test it out. If I do get more testers for v4.0, I'll contact you directly to set something up :)
```

---
## \#90 Posted by: annihil8ted Posted at: 2019-10-02T06:59:04.277Z Reads: 66

```
Sweet, sounds good to me!
```

---
## \#91 Posted by: Chupacabra Posted at: 2019-10-09T23:21:22.604Z Reads: 62

```
Sign me up as well!
```

---
## \#92 Posted by: Ricco Posted at: 2019-10-28T01:00:57.198Z Reads: 49

```
v4.0 of the TTL control module is finished :smiley: This revision packs in a bunch of different improvements. Most are to solve issues found by beta tester, but a few are to add useful features not present in v3.4. For anyone that's curious here's a full list:
1. Added series resistors to UART rx and tx to protect the ESC when the TTL is powered and the ESC is not
2. Replaced the AUX FET with the one from the HPCM so that a horn can be connected directly to the control module
3. Removed the Nunchuck port
4. Made the button port a 3 pin port to match the receiver connections
5. Replaced the boot button with a circuit that puts the module in bootloader mode when the USB is connected, so there is no need to push a button to update FW anymore
6. Changed the micro pins used for UART to allow for auto pin assignment
7. Added pull-downs to all output FETs to prevent LED blinks and horn beeps on start-up
8. Replaced the USB connector with a vertically mounted version for easier FW updates in dense builds
9. Changed the IMU from 9DOF to 6DOF since the magnetometer wasn't being used and it decreases part cost

I'll be ordering some PCBs this week and building up a few prototype boards when they arrive. Once I prove out the new features and fixes I'll call on some memebers that expressed interest in beta testing to start testing with the new boards. If all goes well this will be the final PCB revision before kits are made available :crossed_fingers: 

https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-2/88821/1700?u=ricco
```

---
## \#93 Posted by: venom121212 Posted at: 2019-10-28T13:15:00.092Z Reads: 43

```
Great to hear! Thanks for all your hard work.
```

---
## \#94 Posted by: Pantata Posted at: 2020-01-19T18:47:54.924Z Reads: 17

```
Any updates? Many items not in stock etc... This looks totally awesome!
```

---
## \#95 Posted by: Ricco Posted at: 2020-01-20T17:52:43.274Z Reads: 12

```
Thanks for the support and interest :blush: I am still just starting beta testing of the v4.1 HW. The one thing setting me back at the moment is the power switch I designed for the lighting system which allows you to use the system with ESCs that have an integrated antispark switch. The type of antispark switch used in ESCs varies so I am having trouble designing my switch to work with all ESCs.

I have been focused on the HW side of my projects lately so I haven't gotten time to get the web store of my site tested yet. Once I do I'll start taking orders for my available projects/parts there, but until then I'll be handling orders through PM.
```

---
