# Telemetric Longboard &#124; VESC+ ESP8266+iPhone &#124; old Deck from attic &#124; BLDC Turnigy 6374 149kv&#124; Custom Mount &#124; 12S 5000mAh &#124;

### Replies: 10 Views: 2169

## \#1 Posted by: nick.fisher Posted at: 2017-02-28T06:55:35.614Z Reads: 164

```
Hello I'm Nick from Austria and i would like to present you my first approach of building an electric longboard.

<img src="/uploads/db1493/original/3X/3/1/31cf0ac57361dcb4a48f64ac0d846b0b88fd3580.JPG" width="666" height="500">

**Project Aim:**

* electric Longboard with high enough torque to go up steep hills (>20%)

* easy handling and controlling of the board

* good price to quality ratio

* safety features (limiting current, liming current ascent)

* Display live telemetry data on phone

* Change live board beheaviour on phone

**Concept Longboard**:
<img src="/uploads/db1493/original/3X/8/d/8d965f6eaad2175b6c552cf532a8665ed5df6e0c.png" width="690" height="313">

Used Parts:

* BLDC: Turnigy Aerodrive SK3 - 6374-149kv Brushless Outrunner Motor

* VESC: Enertion VESC-X

* Battery: 3x ZIPPY Flightmax 5000mAh 4S1P 20C

* µC: Selfmade Custom board for ESP8266-01

* Deck+Trucks: old Deck from the attic

* wheels: Enertion 83mm
 
 

**Concept Remote**:
<img src="/uploads/db1493/original/3X/9/a/9a19dff354e08dd1483e0a515ab9dd1574b5114a.png" width="496" height="500">

Used Parts:

* Phone: Iphone 6 (App TouchOSC)

* Remote: Selfmade (Joystick Playstation Portable, ATTiny85, ESP8266,2xAA Battery, Switches and Buttons)

* calculated runtime 40 hours


**Communication Sequence:**

* [Remote] ATTiny85 reads analog Value from Joystick and sends it over the Serial Interface to the ESP8266

* [Remote] ESP8266 gets Joystick Value via Serial Interface and Sends it over WiFi to the ESP8266 on the longboard
* [Remote] ESP8266 reads Pushbutton Value on Digital In and Sends it over WiFi to the ESP8266 on the longboard

* [Phone]  sends and gets Telemetric Value over Wifi from and to the ESP8266 on the longboard

* [Longboard] : ESP8266 on the longboard gets Values from Remote and iPhone and is communicating with the VESC over the Serial Interface.

**Interface Phone:**
Detailed Dashboard with the Information about all measured Parameters:
<img src="/uploads/db1493/original/3X/7/d/7d3daa28c28ab5753b0508c1c430590b555ae553.PNG" width="690" height="387">

Changing of K and T value of the PT1 transfer function for changing the behavieour of the remote: 
<img src="/uploads/db1493/original/3X/5/1/517ff1d32e420e981fd658dedf85953a149b8ea3.PNG" width="690" height="387">

Dashboard:
<img src="/uploads/db1493/original/3X/d/8/d80fefd3102b911bd0f223df250110b5b2a48a99.PNG" width="690" height="387">

**Remote:**
<img src="/uploads/db1493/original/3X/4/1/4183b4a38d35fcefa0d84107d144b2e61e4324a8.JPG" width="375" height="500">
<img src="/uploads/db1493/original/3X/e/f/ef10ad26a2001c5a44434021c092197954089ab0.JPG" width="375" height="500">

**Longboard build:**
<img src="/uploads/db1493/original/3X/3/1/31cf0ac57361dcb4a48f64ac0d846b0b88fd3580.JPG" width="666" height="500">
<img src="/uploads/db1493/original/3X/1/4/14337273efba304012c70565a49dec803774ba2d.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/a/8a6875e994712d88ac3fb8b6503bbb6c5334d14e.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/e/e/eedd28ae46a78646c9a3688e5fc113f247396c4c.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/8/8/88e048370ab94cb57133451144ba747798dae5f8.JPG" width="666" height="500"><img src="/uploads/db1493/original/3X/d/8/d890fc18acb9eae0d34c971a7482802ee10b4556.JPG" width="666" height="500">

If you have any questions or suggestions for improvement please let me know.

Happy e-boarding

Nick
```

---
## \#2 Posted by: kyo Posted at: 2017-02-28T07:14:38.180Z Reads: 132

```
Awesome awesome board man, im interested in the remote, can you tell me more ab it? How did you make it?
```

---
## \#3 Posted by: nick.fisher Posted at: 2017-02-28T07:23:35.128Z Reads: 139

```
For the remote I just used a psp-joystick like this one: [https://www.adafruit.com/product/444](https://www.adafruit.com/product/444)
and  I used an ATTiny85 microcontroller to read the analog values of each axis. After digitizing the input the ATTiny sends via the serial interface to the esp8266. The esp8266 is connected to the esp8266 on the longboard, which works as accesspoint and sends the data via udp protokoll. So in the remote are two programmed microcontrollers.
Here are the layout and scheme:

<img src="/uploads/db1493/original/3X/7/1/716aa37a8f4c3ca4d080270d756a5a99f5d604d0.PNG" width="690" height="205">
<img src="/uploads/db1493/original/3X/3/2/3286a81b925f458810826bdf2d81b67128533d59.PNG" width="690" height="384">

 I hope I've answered your question
```

---
## \#4 Posted by: Journ Posted at: 2017-02-28T09:29:55.079Z Reads: 114

```
What happens when you get out of Wi-fi range or did i misread that it needs Wi-fi for the phone and joystick remote?
```

---
## \#5 Posted by: nick.fisher Posted at: 2017-02-28T09:52:47.769Z Reads: 112

```
Usually the board can't get out of Wifi range, because the board broadcasts it's own Wifi. So you moving your accesspoint with the board.

But in case that there is any connection error or timeout of a component (phone, remote, vesc), the board is set to a save  state with a braking current of 10A. To get out of the save state there is the button "arm" on the phone
```

---
## \#6 Posted by: PXSS Posted at: 2017-02-28T11:45:44.536Z Reads: 104

```
I suggest you instead make it go to zero throttle and let it coast. Otherwise you might find yourself flying off the board if you lose connection at high speed
```

---
## \#7 Posted by: IsTalo Posted at: 2017-02-28T12:37:26.859Z Reads: 97

```
You could use a Wii remote with the Esp8266, it's safety
```

---
## \#8 Posted by: nick.fisher Posted at: 2017-02-28T12:47:19.992Z Reads: 91

```
I havn't experienced any connection issues so far, except the ones I've provoked for testing the safety mechanism. 

In case of a connection loss I first set to zero throttle and then a soft ascend of braking, so the change of momentum isn't too rapid.
```

---
## \#9 Posted by: Ackmaniac Posted at: 2017-02-28T14:53:20.285Z Reads: 85

```
I also experimented with the ESP8266 and i can't recommend to use it for throttle inputs. 
Disadvantages are also the high current consumption of around 100 mah (at the remote).

I also have the small joystick that you use and i can't imagine that it is sensitive enough for throttle inputs.
You also don't necessarily need the ATTiny85 in between. You could detect both axis via one ADC pin. But as i said already the joystick from the PSP that you use isn't precise enough. Also the resistance for the thumb is very low which would make it hard to find the right position for the right amount of power.
```

---
## \#10 Posted by: nick.fisher Posted at: 2017-02-28T15:32:30.844Z Reads: 83

```
Thank's for the feedback.

The psp joystick for the remote isn't perfect but i had some of them lying around and therfore I used them. Concerning the esp8266 and the analog input. I'm using a ESP8266-01 and the ADC Pin isn't accessable via the pinheader and i won't use some fiddly soldered wires directly to the chip. 

For the better respone-behavior I programmed a PT1-Transfer function for filtering the input signal and as result i get a quite natural feeling throttle behavior. With this PT1 filter the exact position of the thumb isn't necessary any more.

The power consumption isn't that important to me, I've experienced a battery life of the remote of about 40h.
```

---
