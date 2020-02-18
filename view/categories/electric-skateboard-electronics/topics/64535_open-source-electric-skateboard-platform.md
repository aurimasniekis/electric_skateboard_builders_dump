# Open Source Electric Skateboard Platform

### Replies: 17 Views: 1947

## \#1 Posted by: Skyng22003 Posted at: 2018-08-11T10:01:19.228Z Reads: 221

```
Hello everyone,

I've have been working on an opensource electric skateboard platform for a few years, I think I started this project before Boosted Boards Kickstarter.

I have now built and tested 3 major prototype revisions and feel that the project is mature enough to gauge the communities interest and engage with potential beta testers.

The platform consists of the following parts:

**Main Controller** 
2x ESP32 modules supporting Bluetooth 4.2 and WIFI with modified 16MB flash
Supporting Bluetooth Remote and potentially a smartphone app
Bluetooth bonding, encryption and MITM protection supported
Programmed on the esp32 Arduino core for maximum accessibility
OTA programming over wifi and Telnet command console
The main ESP32 is responsible for communicating with the Bluetooth controller, IMU via I2C and VESC via UART
The sub ESP32 is responsible for data logging, communicating with the LIPO charge controller, BMS and electronic fuse.

USB Hub for ESP32 programming and VESC USB passthrough

SD card slot for data logging

MPU9250 IMU for torque vectoring and orientation sensing
![IMG_20180811_092007|666x500](upload://sOzF0mKcG6NtfoI2AV4a62WWfbW.jpg)
![IMG_20180811_092043|666x500](upload://7CQWwTnuYAaHD9SjKhKlPK0TpJm.jpg)

A previous version of the Main Controller running 2x STM32F3 MCUs, has NFC built in however the anntenna wire required was too long so the NFC read was not realiable
![IMG_20180811_085259|666x499](upload://fcmUb5KHtihZGYerd90jxZy3IOq.jpg)
![IMG_20180811_085317|375x500](upload://j7g0tBaD108nKAWy09BFjaNsrdp.jpg)

**BLDC Controller**
2x VESC v4.12, firmware based on fw 2.18
I have added additional packet types so that only essential information is sent to and from the ESP32 which reduces latency and increases refresh rate.

BQ24610 LIPO charger supports up to 6S and 10A

LT8640 DC-DC regulator outputs 3.3v up to 5A provides power to the Main Controller board and the VESC microcontrollers 

LTC2951 soft power on switch/reset controller 

![IMG_20180811_085655|375x500](upload://lerua0NCSgYtoU498acXEtRVBwI.jpg)
![IMG_20180811_085736|375x500](upload://qhfuz09OSmOd2CerFKzNSy97Ban.jpg)
![IMG_20180811_085826|375x500](upload://9pBWJYwS9X0aQYeh77Bth6QuX9Y.jpg)
**Remote Control**
Infinite scrolling controller
The total power draw with the screen on and Bluetooth transmitting is under 15ma  
DA14583 M0 Cortex and BLE 4.2 SOC
Bluetooth bonding, encryption and MITM protection supported
Programmed on the SemiDialog SDK which is C, unfortunately, I could not find any SOC that comes close to this one that supports Arduino
As far as I know, there are currently no SOC as low power or as compact, which will allow a wide range of controller form factors in the future.

96x16 OLED Screen

LTC2951 soft power on switch/reset controller 

Haptic feedback motor

MCP73831 LIPO charge controller

Induction charging support
![IMG_20180811_084436|375x500](upload://5KSSm1u75Cbtb7W6ryWu5jGOifC.jpg)
![IMG_20180811_090631|375x500](upload://4bVN1fei4nOMxMPqtETrnWD9a6q.jpg)![IMG_20180811_090650|375x500](upload://11BR3xt5zrCDoTSs9eAIwF7QHIu.jpg)

A previous prototype with DA14580
![IMG_20180810_084047|375x500](upload://2AL0h2trvNyi8OyzciyZh5sufwa.jpg)

**BMS**
BQ76PL36 cell balancing up to 6S, this is stackable for more cells (Tesla uses the same controller in their battery packs)

The only one I built is inside my battery pack so I'm only showing the PCBs
![IMG_20180811_090210|375x500](upload://goQGrMcqI2A0ZE8Wnn87EgZeeNT.jpg)

**Electronic Resettable Fuse**
Programmable trip current via I2C, no microcontroller all functions carried out at using simple transistor logic
4x IRFS7530
LT1910 high side MOSFET driver
ACS756 current sensor
LM393 voltage comparator which turns the LT1910 on/off based output from ACS756
2x AD5259 I2C digital potentiometer for adjusting trip current

The only one I built is inside my battery pack so I'm only showing the PCBs and this part still requires additional testing

![IMG_20180811_093325|375x500](upload://3Pkf6Tj5uVisTrn7gDZ8GGpULI4.jpg)![IMG_20180811_093338|375x500](upload://td8H6amSGIXoUib7BBeTejgHvN9.jpg)

**My current setup**
I've been using this as a daily commute for a while hence the dents and sratches
![IMG_20180811_091326|375x500](upload://yZMwLSNE7bPvMhTqrXLCDwZCt0N.jpg)
![IMG_20180811_091348|666x500](upload://ff7R58YW60oSVzWKStinNzzyNE2.jpg)

Back panel containing the Bluetooth/WIFI antennas, magnetic charge port and USB programming port
![IMG_20180811_091040|375x500](upload://kBeLPaQboYfRkxizdJBaUDKr0qO.jpg)

Thank you for your attention let me know your thoughts below!
```

---
## \#2 Posted by: pat.speed Posted at: 2018-08-11T11:55:24.185Z Reads: 177

```
This is a pretty cool project and congrats on putting so much work into it. It would be cool if the battery module could do up to 13s though as many boards now use higher voltages
```

---
## \#3 Posted by: solodros Posted at: 2018-08-11T12:25:33.341Z Reads: 172

```
Great job, look forward to your sharing
```

---
## \#4 Posted by: Jc06505n Posted at: 2018-08-11T12:27:11.761Z Reads: 170

```
Awesome , how does controls Via ring feel?
```

---
## \#5 Posted by: Skyng22003 Posted at: 2018-08-11T13:25:02.265Z Reads: 162

```
Thanks, the BMS can be stacked and can easily support up to 192 cells so that's the easy part.

Supporting 14s charging might be more difficult but can be done with IC's such as MC33771.

I understand 14s is the max voltage the VESC can take.

I'll put it in my next revision, if someone has a better way of doing this please let me know.
```

---
## \#6 Posted by: Skyng22003 Posted at: 2018-08-11T13:37:22.793Z Reads: 153

```
I think you get finer control of the acceleration and braking as it is not limited to 180 degrees. It is also immune to sudden acceleration and braking as you do not have to keep you finger on the ring. It uses a safety switch to go between acceleration/braking and coast mode.

Holding down the safety and scrolling up to accelerate, scrolling down decreases the amount of acceleration, past the coast point switches to braking. To quickly switch to braking release and reengage the safety and scroll down.  

The ring controller is just an example of what can be done with the DA14583, you could build any type of controller you can think of using that platform.
```

---
## \#7 Posted by: Skyng22003 Posted at: 2018-08-11T13:39:52.415Z Reads: 140

```
Thanks, I'm hoping individuals will join the development and create an open source and user-friendly platform,
```

---
## \#8 Posted by: okp Posted at: 2018-08-11T14:01:32.069Z Reads: 131

```
congrats for such dedication. Keep it going man.
```

---
## \#9 Posted by: 12meterkuk Posted at: 2018-08-11T14:23:54.163Z Reads: 128

```
That remote looks like the original design from the boosted Kickstarter! Did you work with them on it perhaps?
```

---
## \#10 Posted by: Skyng22003 Posted at: 2018-08-11T15:07:03.991Z Reads: 132

```
Nope, I didn't work with them.

It's one of the ideas that I had early on, I guess it's a coincidence, but back in 2010 there was no way that the ring controller could be built due to the battery constraints, I had a similar design with a much longer tail but due to the battery drain it would only last 1-2hrs so I shelved the idea. I was actually very curious to see how the team at Boosted would pull it off, clearly, they also couldn't make it viable. 

In the meantime, I worked on other controllers like this glove controller below.
![IMG_635517449491825530|375x500](upload://r5azJtc6NCbmk0PsE8byHL1DVyw.jpg) 

But once the DA14580 was released I started working on the ring controller again as the glove controller was a bit too fiddly to implement reliably.
```

---
## \#11 Posted by: ggalisky Posted at: 2018-08-11T16:39:15.966Z Reads: 118

```
This is really inspiring stuff. I'm working on my electrical engineering degree right now, so I don't think I would be of much help. I have just started learning Eagle for designing circuits though. At any rate if you need any testing or help with the project let me know.
```

---
## \#12 Posted by: mishrasubhransu Posted at: 2018-08-11T17:57:46.799Z Reads: 110

```
What trucks are those?
```

---
## \#13 Posted by: Vanarian Posted at: 2018-08-11T20:05:53.398Z Reads: 101

```
Nice work man, keep it up!
```

---
## \#14 Posted by: Skyng22003 Posted at: 2018-08-16T20:52:56.876Z Reads: 70

```
That's great! I have no formal electrical/mechanical engineering training myself so don't limit yourself as to what you can achieve. I think KiCad is much easier to use in my opinion, give it a shot if you have time. 

Thanks for the offer! I'm working on some code to run on a off the shelf ESP32 dev board which has a screen and LIPO charging circuits to use as a remote, see this thread
https://www.electric-skateboard.builders/t/remote-design-based-on-esp32/64333/56  

If you have a skateboard build and are happy to test out the remote/receiver pair that would be great!

I'll be rewriting some code from my current build to run on a single ESP32 to control the VESC
```

---
## \#15 Posted by: Skyng22003 Posted at: 2018-08-16T20:53:28.784Z Reads: 62

```
I designed them and got them CNCed :grin:
```

---
## \#16 Posted by: Skyng22003 Posted at: 2018-08-16T21:08:44.350Z Reads: 60

```
Looking into @pat.speed suggestion I think this LIPO charger would fit the bill
http://www.analog.com/en/products/ltc4020.html

It's a buck-boost charger capable of supporting battery packs up to 55volts

Am I correct in thinking most people who use high voltage pack use LifePO4 chemistry?

So at 14S it would be 3.6x14=50.4V

One advantage of this charger IC is that it has a boost mode which means that your AC adaptor can have a lower voltage than your battery pack, which I think will be very convenient.

The issue I am tackling now is what is the best way to set the charge voltage as different people would have different pack voltages, would people be happy to solder on the correct resistors to set the charge voltage or would a digital potentiometer implementation be better?

The only issue I can see with using a digital potentiometer is if someone hacks the controller they can change the charge voltage and blow up the LIPO pack.

@ggalisky What do you think?

Please let me know if any of you have thoughts on this issue
```

---
## \#17 Posted by: ggalisky Posted at: 2018-08-17T02:28:05.855Z Reads: 48

```
I have a boosted inspired board, 10s4p Samsung 30Q, dual focbox and torqueboard 6355 motors. I’d be happy to test and record data on parts for this project. Feel free to PM me.
```

---
