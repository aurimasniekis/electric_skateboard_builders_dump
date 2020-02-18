# LED strips connected to the board

### Replies: 26 Views: 670

## \#1 Posted by: fredrikinn Posted at: 2019-04-30T21:54:50.562Z Reads: 167

```
Hi i got some new LED strips i wanted to connect to my elongboard. I tryed to connect them to my rc reciver (the reciver for my controller). It works fine and i can turn the lights on and off using a switch on the remote. The problem is that the LED lights dont get enough power so they light up pretty badly. Any ideas how i can do this? want to be able to turn the lights on and off with the remote. 

extra question: I have a SP110E LED Hue bluetooth controller for the light. Any good Apps i can use to get half the leds white and the other half red?
```

---
## \#2 Posted by: Mich21050 Posted at: 2019-04-30T21:56:39.838Z Reads: 169

```
Just one quick search will reveal that there are a bunch of options on here...\
For example:\
https://www.electric-skateboard.builders/t/pwm-controlled-brake-light-controller-open-source/85588\
https://www.electric-skateboard.builders/t/beta-testers-needed-teltail-lights-ttl-interactive-eskate-lighting-system/86912
```

---
## \#3 Posted by: mmaner Posted at: 2019-04-30T21:59:36.988Z Reads: 140

```
Do a search for buck converter and step-down converter and you will see a lot of examples.

https://www.electric-skateboard.builders/search?q=buck%20converter
```

---
## \#4 Posted by: fredrikinn Posted at: 2019-04-30T22:04:38.330Z Reads: 138

```
A buck converter steps down voltage dosent it?
```

---
## \#5 Posted by: Mich21050 Posted at: 2019-04-30T22:05:39.062Z Reads: 140

```
Yes it does.
```

---
## \#6 Posted by: fredrikinn Posted at: 2019-04-30T22:10:27.955Z Reads: 133

```
How would that help me when i need more?
```

---
## \#7 Posted by: Mich21050 Posted at: 2019-04-30T22:10:49.267Z Reads: 126

```
Whatcha mean?
```

---
## \#8 Posted by: fredrikinn Posted at: 2019-04-30T22:14:43.461Z Reads: 117

```
when i connect the led strips to the rc reciver the light gets under 5v. The LED strips barely lights up
```

---
## \#9 Posted by: rusins Posted at: 2019-04-30T22:48:42.424Z Reads: 112

```
Because your lights are using a lot of current, the receiver (actually the ESC powering the receiver) isn't powerful enough to maintain the 5 volts you need. Using a step-down converter directly from your battery will make sure your lights have enough power without dropping below 5V :slight_smile:
```

---
## \#10 Posted by: fredrikinn Posted at: 2019-04-30T23:09:35.482Z Reads: 111

```
Any way to use my remote controller ch2 as on/off switch when i use a step-down converter directly connected to the battery?
```

---
## \#11 Posted by: rusins Posted at: 2019-04-30T23:12:42.018Z Reads: 113

```
Yes, a transistor and a resistor so that the receiver toggles power in the step down converter circuit. Others have probably done it on this forum before with a better explanation, but here's what I did for my brother's board:

![photo_2019-05-01_00-11-06|666x500](upload://ngr2PRaXhSBFBxZn8rV8XRXbo11.jpeg) 

Left side would be the output of your step down converter, and right side is channel 2 of your receiver :slight_smile:

For me the lights still faintly glow even when the remote isn't turning the transistor on, so I guess I picked a bad transistor :confused:
```

---
## \#12 Posted by: Ricco Posted at: 2019-04-30T23:35:53.193Z Reads: 101

```
You can use an RC switch like this one to switch the power from the step-down converter to your LEDs

https://hobbyking.com/en_us/turnigy-receiver-controlled-switch-1.html?countrycode=US&amp;gclid=Cj0KCQjw5J_mBRDVARIsAGqGLZD6JYa6OFhAngokterTjzc_9trZH5QixAhkE9fsx0fcv8jmX21Ekl4aAlyeEALw_wcB&amp;gclsrc=aw.ds
```

---
## \#13 Posted by: MD84 Posted at: 2019-04-30T23:46:02.229Z Reads: 99

```
This is my solution:
![1556667494031620650291558346257|690x388](upload://5ODLeYMvXJfXcdinagUYU8264w1.jpeg) 

![15566675518376527261685657308537|690x388](upload://6A0PR3t6DXnyd7kuoFK7QBLNB4z.jpeg)

![15566680728301838100167125382244|281x500](upload://5uiVAaNbEnTY5jJbKnL1JfOMTgo.jpeg)

I just temp wired it last night...

I am using Arduino nano powered off receiver. 40T provides power to LEDs. Channel 2 (steering) provides data input to arduino. Arduino provides data out to switch on LEDs and change colors/patterns based on channel 2 pot position. 

Battery tube can swap 21700 or 18650 as necessary. One 40T should power the 64 nodes for minimum 3 hours.

Battery tubes can be assembled multiples in series to series more batteries. The DC barrel jack head can be swapped for an LED headlight, high power connector....etc, it's modular...

![15566686355475607715827628291471|690x388](upload://bvaSl5y192ocm5BYGfKdU1goaNk.jpeg)
```

---
## \#14 Posted by: ZachTetra Posted at: 2019-05-01T00:23:05.740Z Reads: 90

```
I may have gone overboard on LEDs planning out for...144 addressable LEDs running off the main battery and another 6x T6 LEDs on a light bar.  A car high beam is about 1200 lumens, this is about 6000 lumens total
```

---
## \#15 Posted by: Movation Posted at: 2019-05-01T00:39:17.387Z Reads: 89

```
I use these buck boards puts out 4 amps, Run my 5 volt headlights, WS2815 strips driven by my nano firefly variant receiver ESP32-lora (Droid), and brake lights and I also breakout a waterproof USB to the side of my enclosure to use to charge my phone, transmitter, tablet.
https://www.banggood.com/DC-DC-7-60V-To-5V-5A-4USB-Output-Buck-Converter-Step-down-Power-Supply-Module-p-1229015.html
They even work with my 13S Board
```

---
## \#16 Posted by: MD84 Posted at: 2019-05-01T01:31:20.158Z Reads: 79

```
How does the waterproofing USB work? Do you need to silicone it in or does it provide some sort of sealing gland or otherwise?
```

---
## \#17 Posted by: Movation Posted at: 2019-05-01T02:30:54.580Z Reads: 82

```
https://www.aliexpress.com/item/USB-Female-Socket-Plug-Panel-Mount-Adapter-Waterproof-Connector-IPL7-With-Cap/32912079378.html
then you use a 12"  male to male usb to connect to the buck converter
https://www.aliexpress.com/item/New-30cm-Blue-USB-2-0-Type-A-Male-To-USB-Male-Adapter-Blue-High-Quality/32822614483.html
I also use a micro usb version and a 4 way toggle switch (master/Slave) and 2 x 90 degree male microusb plugs for programming my duel vesc without opening my enclosure 
https://www.aliexpress.com/item/Micro-USB-2-0-IP67-Waterproof-Cable-Micro-USB-5pin-IP-67-Male-to-Female-Panel/32953801137.html
```

---
## \#18 Posted by: legend27 Posted at: 2019-05-01T05:51:01.085Z Reads: 76

```
I used a step down converter and just a switch. Would be cooler if I could turn on/off the led with my remote like you.

![image|666x500](upload://p837pLsSD12xF3oMiBoDt7Gek6V.jpeg)
```

---
## \#19 Posted by: fredrikinn Posted at: 2019-05-01T08:39:50.998Z Reads: 70

```
Thanks for all the help :smiley:

Anyone know how i can change set the led lights color? want half the leds white and the other half red. The app i use now only allow me to set a solid color and it has a few presets, blinking in different colors. But nothing like i want it 

The App i use now: 

![image|252x432](upload://2LO6drrwkF1rvosXrIivtBemDZ8.jpeg)
```

---
## \#20 Posted by: chickengun Posted at: 2019-05-01T11:22:03.271Z Reads: 68

```
Always keep in mind that there will be heat created by any step down converter. I used [this](https://www.aliexpress.com/item/1pcs-Original-Hobbywing-UBEC-5A-HV-Switch-Mode-UBEC-High-Voltage/32757601350.html) ubec in combination with my 10s4p battery pack to power 60 WS2812B leds. It acts as a step down converter but at the same time provides a clean 5V source. I use a chinese led strip where the max power consumption is 0.5 A at 5 V for 60 leds (all leds white) and the ubec warmed up to 40 °C. On avarage it's something between 0.3-0.4 A
```

---
## \#21 Posted by: MD84 Posted at: 2019-05-08T04:40:20.051Z Reads: 54

```
This is why I like to run a single cell li-ion for a dedicated lighting battery. No heat, no loss, no additional load on main battery.
```

---
## \#22 Posted by: J0ker3366 Posted at: 2019-05-08T05:51:36.301Z Reads: 55

```
[quote="fredrikinn, post:19, topic:92370"]
want half the leds white and the other half red.
[/quote]

This is only doable if the led strips have RGB connections on them. If all you have is single red and black connections, then you cant, afaik. You might be able to see about a 2-channel led controller
```

---
## \#23 Posted by: fredrikinn Posted at: 2019-05-09T11:03:04.847Z Reads: 45

```
I have this LED:
https://www.ebay.com/itm/WS2812B-Strip-LED-Lights-5050-RGB-30-60-144-LED-M-IC-Individual-Addressable-DC5V/223222365145?ssPageName=STRK%3AMEBIDX%3AIT&amp;var=522018470617&amp;_trksid=p2060353.m2749.l2649
And this controller:
https://www.ebay.com/itm/2Pcs-Bluetooth-LED-Remote-Control-Controller-SP110E-For-WS2811-RGB-LED-Strip/173408761372?ssPageName=STRK%3AMEBIDX%3AIT&amp;_trksid=p2060353.m2749.l2649

Should work then, right?
```

---
## \#24 Posted by: MD84 Posted at: 2019-05-09T14:36:49.797Z Reads: 42

```
You will be limited to the color and pattern options of the controller. If there is not a setting for what you want on the controller you are out of luck. Unless the controller is programable some way. 

This is why I like to use an Arduino. Your light pattern possibilities are endless. I think I'm going to make a police light pattern and try to sell an esk8 to my local police department.
```

---
## \#25 Posted by: Movation Posted at: 2019-05-10T05:23:02.271Z Reads: 35

```
With an Arduino its easy to link the speed of the LEDS scroll with board speed, Bright red for breaking. I use my receiver (esp32) its quick enough to run the neopixel code & control my skateboards. I am planning on doing a colour change based on battery state @ 30% leds will change to orange @ 20% leds will change to red
```

---
## \#26 Posted by: MD84 Posted at: 2019-05-10T09:55:49.506Z Reads: 28

```
This is a good idea. We're you planning on a simple resister voltage divider from the battery to an Arduino input? I use the fastled library, haven't tried neopixel. 

I am assuming you are using the the throttle output from your receiver for breaking vs actual speed. If we had actual speed input I wonder if we could do some cool lighting effects where the pixel movement was inversely correlated to speed.
```

---
