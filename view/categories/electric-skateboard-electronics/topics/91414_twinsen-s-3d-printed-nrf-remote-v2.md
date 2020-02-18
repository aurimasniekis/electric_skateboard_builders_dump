# Twinsen’s 3D Printed NRF Remote v2

### Replies: 3 Views: 1064

## \#1 Posted by: Twinsen Posted at: 2019-04-22T16:40:36.624Z Reads: 141

```
This is an updated and a better organized topic about my esk8 remote, an improved and customized version of [solidgeek’s remote](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/) and [ervinelin’s remote](https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231/).

![IMG_1343|666x500](upload://ohPArELgO3Yn7k1GJ1WED2eju8g.jpeg) 
![IMG_1353|666x500](upload://bLxdQNRfzrlxq5jxkh7aoQpCFsv.jpeg) 

**Features:**

* Trigger style remote with long stick travel.
* Cheap to build, with easy to find parts from aliexpress.
* OLED display showing board battery voltage and distance remaining.
* Battery voltage sensor in the receiver that can measure 0 to 51v.
* Automatic distance calculation based on LiPo or LiIon discharge curves.
* Two PPM outputs for connecting regular ESCs or VESCs.
* Dead man switch that prevents accidental throttle.
* Setting menu to set display rotation, Throttle and brake endpoint, Smooth braking and acceleration, and other settings.
* Cruise control with smooth acceleration.
* 5 meter RF range.
* RF collision avoidance when using multiple remotes, autobinding algorithm. Selectable RF channel.
* Carefully written and tested code with many fail-safes in place to avoid any injuries.
* 20+ hours battery life on one charge.
* Internal micro-usb charger.

**Not implemented:**
* VESC telemetry support

I don't have VESCs in my mountainboard so I can't properly test that functionality. If anyone is willing to send me 2 VESCs I'll send back a fully assembled remote and implement telemetry support (speed, amps, etc) :)

### Links so you can make your own:

Schematics:

Transmitter: [https://easyeda.com/Twinsen/nrf-remote-2 ](https://easyeda.com/Twinsen/nrf-remote-2)

Receiver: [https://easyeda.com/Twinsen/NRF-Remote-2-receiver ](https://easyeda.com/Twinsen/NRF-Remote-2-receiver)

3D printing files:
[https://www.thingiverse.com/thing:2843488 ](https://www.thingiverse.com/thing:2843488)

Parts list:
[https://docs.google.com/spreadsheets/d/1Ayte5Xm0up_AQHfdTZghDGnGC5o7WZZo4H4hzZ2LCAw/edit?usp=sharing ](https://docs.google.com/spreadsheets/d/1Ayte5Xm0up_AQHfdTZghDGnGC5o7WZZo4H4hzZ2LCAw/edit?usp=sharing)

Code:
[https://github.com/asafteirobert/nRF24-Esk8-Remote ](https://github.com/asafteirobert/nRF24-Esk8-Remote)
### Pictures
[details="click to expand"]
![IMG_1338|666x500](upload://nIP99UjAIzQyTWH3ZF62fuvbPLw.jpeg)
![IMG_1339|666x500](upload://zxRiWwj1IDapgP6RlgzlpQWyRmc.jpeg)
![IMG_1340|666x500](upload://k2Qo9FZk9LNRuKbVH7mk8Cm9GPI.jpeg)
![IMG_1341|666x500](upload://cqXWPAkPfI8h3vuXaJzKMPg4B1m.jpeg)
![IMG_1345|666x500](upload://d2n9xYIROFgl3toLLVyA9GR7ZKn.jpeg) 
![IMG_1348|666x500](upload://ahTDsCnHheKL8bdusU6hLJnzVsf.jpeg) 
![IMG_1350|666x500](upload://y8xN5eD4nphjeSjDLmgEAxFih7C.jpeg) 
![IMG_1355|669x500](upload://soRJFg2DzHDZkJt3wS9UL50Mpj6.jpeg) 
[/details]
### Usage Documentation:
[details="click to expand"]
__Settings__

Press and hold the Dead man switch while the remote is starting to enter the settings menu. Use the Page switch button to navigate the settings. Some setting use the Cruise control button for special actions. Each setting is saved to EEPROM when you press the Page switch button.
[details="Settings table (click to expand)"]
|Setting|Default|Range|Description|
| --- | --- | --- | --- |
|Rotate Display|False|True, False|Rotate the display, so you can use the remote in the other hand. Setting takes effect after restart.|
|Battery type|||The battery type that is connected to the receiver voltage sensor. Used for calculating the battery level in the "BATTERY" page.|
|Battery cells|10s|0-12S|The cell count of the battery that is connected to the receiver voltage sensor. Used for calculating the battery level in the "BATTERY" page.|
|Throttle deadzone|2%|0-50%|How much of the stck travel is ignored in the center.|
|Throttle min|150|0-1023|Hall sensor value for minimum throttle. Move your stick to the maximum brake position and press the Cruise control button to automatically set the value.|
|Throttle center|512|0-1023|Hall sensor value for middle throttle. Leave your stick to the idle position and press the Cruise control button to automatically set the value.|
|Throttle max|874|0-1023|Hall sensor value for maximum throttle. Leave your stick to the maximum throttle position and press the Cruise control button to automatically set the value.|
|Brake endpoint|100%|0-100%|The end point of the braking value. Set it lower to have softer brakes|
|Thr. endpoint|100%|0-100%|The end point of the throttle value. Set it lower to have smaller maximum throttle.|
|Brake accel.|0sec|0-5sec|Braking acceleration time: The number of seconds it takes to reach 100% brake. Set it to as low as possible so when slamming the brakes you don't land on your face. Set to 0 to disable. USE WITH CAUTION: This makes brakes respond softly, so use small values and make sure you test that you are always able to stop in time.|
|Throttle accel.|0sec|0-5sec|Throttle acceleration time: The number of seconds it takes to reach 100% throttle. Set it so when you slam the throttle you are not thrown off the board. Set to 0 to disable.|
|Cruise accel.|1sec|0-5sec|Cruise control acceleration time: The number of seconds it takes to reach 100% throttle when using cruise control. Set it so you comfortably accelerate towards the desired cruise control value. Set to 0 to disable.|
|Voltage cal. sen.|1|0-2|Voltage calibration multiplier for the receiver sensor: Multiplies the voltage of the receiver sensor with this value, to calibrate it.|
|Voltage cal. rem.|1|0-2|Voltage calibration multiplier for the remote battery: Multiplies the voltage of the remote battery sensor with this value, to calibrate it.|
|Batery range|10KM|0-99KM|The typical range you get on a battery, used to calculate the remaining range on the "DISTANCE" page.|
|Radio Channel|108|0-125|The radio frequency used for communication. Change to avoid interference when using multiple remotes nearby.|
|RESET ALL|||Press the Cruise control button to reset all settings to default|
[/details]

__How cruise control works:__

Cruise control will remember a set throttle value and it will send that throttle value as long as the button is held down. Braking still works even is the cruise control button is held down. The dead man switch needs to be held down even during cruise control.

To set your cruise throttle, move the stick to the desired throttle position and then start holding down the Cruise control button. You can now release the stick and the throttle value will be maintained. If you start pressing the Cruise control button while the stick is in idle position, you will accelerate to the last value you set.

If while holding the Cruise control button, and your stick throttle value is larger than the cruise throttle, the stick throttle will be used instead. This way you can temporarily give extra throttle when cruising.

__Pages__

Battery: Shows the voltage of the battery connected to the receiver sensor. The progress bar shows the percentage of the battery level. The percentage is calculated based on the typical discharge curve of the battery type selected in the settings. Remember to also set the correct number of battery cells.

Distance: Shows the remaining range of the battery. This is just a convenience calculation, simply calculated by multiplying your battery level with the battery range from the settings.

Output: Shows the signal sent to the receiver. Recommended to be left on when first using the remote to understand how acceleration, endpoints and cruise control work.

__How binding works__

To avoid conflicts with other remotes, the transmitter and receiver have to be binded. The remote implements autobinding, meaning the transmitter will automatically connect and bind to the first unconnected receiver it detects. The binding code is generated automatically when the remote is first started or when the radio channel setting is changed. To avoid further interference when using multiple remotes, you can use the radio channel setting to change the radio frequency used.
[/details]

### Build Instructions
[details="click to expand"]
Making your own should be pretty straightforward if you follow the links above and look at the pictures. Nonetheless here are some instructions and tips:

* Get all the parts from the parts list.
* 3d print the plastic parts. Some tolerances are quite tight and important. Make sure all the mechanical parts fit and move well. Adjust your slicer's horizontal compensation otherwise. Some parts also need to be rotated.
* Make the PCBs. Use small thickness PCBs, I used 1mm ones. The PCBs are one sided. I etched them myself, so if you plan on ordering them please double check that there are no problems such as missing holes, missing masks, problematic silkscreen, etc.
* Upload the firmware to the Arduino's using the Arduino IDE. You can do this easily without soldering by holing a pin header at an angle on the programming pins.
* Solder components to the PCBs. All components should be in the parts list. The NRF module is extremely close to some solder joints. Make sure it's insulated properly with double sided tape. Make sure the Arduino board sits directly on the PCB; if you use a pin header as a spacer, the module might not fit correctly.
* Finish assembling the receiver by placing it in the case and screwing in the 4 screws.
* Place the LiPo charging board in the transmitter and solder the 4 wires to it. You can use spring contacts for the battery or _carefully_ solder the wires directly to it.
* Solder the wires to the rocker switch, bend the contacts of the switch so they don't touch the LiPo charging board. Insulate the switch so the contacts do not touch the PCB which is added next.
* Place the assembled transmitter PCB in the remote and screw in the 3 screws holding it.
* Attach wires to the Hall sensor, OLED screen and the 3 switches.
* Glue in the Hall sensor, OLED screen and the 3 switches.
* Glue the dead man switch cap to the micro switch.
* Place the bearing inside the trigger plastic part, use a bit of glue on the sides to hold it in place.
* Solder all the wires to the square pads on top of the PCB. Refer to the schematic+board for the correct connections.
* Power it on for the first time and check that the display and buttons work correctly. Set the active page to "output".
* Place the magnets inside the trigger part. They need to be in opposite directions and placed correctly otherwise your throttle will be in reverse. Check that you placed them correctly by checking the screen.
Adjust the position of the magnets so the throttle response is roughly linear (don't worry about the endpoints yet). For 5*8mm magnets, they should be as high as possible.
* Place the lever and spring and make sure everything moves smoothly. Use a bit of glue on the part holding the bearing.
* Go to the settings menu and calibrate the throttle min/center/max values. Adjust the position of the magnets if necessary.
* Place the final top part and screw it in.
* You're done. Double check every function.  Your safety depends on it.
[/details]
```

---
## \#2 Posted by: brenternet Posted at: 2019-04-22T17:18:28.352Z Reads: 106

```
More options :heart:
```

---
## \#3 Posted by: Mich21050 Posted at: 2019-04-30T19:28:14.380Z Reads: 69

```
[quote="Twinsen, post:1, topic:91414"]
I don’t have VESCs in my mountainboard so I can’t properly test that functionality. If anyone is willing to send me 2 VESCs I’ll send back a fully assembled remote and implement telemetry support (speed, amps, etc) :slight_smile:
[/quote]

Nice project. Where do you live? I could send you an mt vesc... :slight_smile:
```

---
