# Twinsen&rsquo;s 3D Printed NRF Remote

### Replies: 28 Views: 3449

## \#1 Posted by: Twinsen Posted at: 2018-03-28T20:12:05.462Z Reads: 384

```
I built my electric mountain-board, so I wanted to make a custom remote for it.

I saw [solidgeek's remote](https://www.electric-skateboard.builders/t/simple-3d-printed-nrf-remote-arduino-controlled/28543/) and then [ervinelin's remote](https://www.electric-skateboard.builders/t/diy-trigger-style-remote-with-telemetry-complete-guide/48231/).
I continued on that work and made my own, based on ervinelin's 3D files and solidgeek's code, with my own simplified schematic.

My my electric mountain-board uses RC ESCs and not VESC's, so for now it does not support VESC telemetry, so if someone can look into it and test it, please do.
The remote uses an Arduino Pro Mini 3v3, 128x32 OLED display, OH49E hall sensor and nRF24L01+ radio module. It's powered by a swappable 18350 lithium battery that can also be charged using the internal USB charger.
It has 3 switches:
1. Dead man switch. This needs to be held down in order to accelerate.
2. Page switch. Used to go through the settings menu and to change the information displayed on the screen.
3. Cruise control button. Hold this down to use cruise control.

The receiver uses an Arduino Pro Mini 5V and nRF24L01+ radio module. It has a voltage divider to measure voltages from 0 to 51v.
It has 2 PPM (PWM) outputs for connecting 2 ESCs, one battery voltage sensor and one UART connector for VESC telemetry, once that is added to the code.

For more detailed information about the firmware features, see the github page.

The nRF24L01+ module I use does not have any range to brag about, but I used it with no problems, dropouts or disconnects for 50km. 
Due to the simplified schematic and it's low power consumption the transmitter battery should last about 20 hours on one charge.

I might be willing to sell 2 or 3 of these in one month. Mostly for fun and to help out the community, since it takes about a day's work to put it together.

![IMG_0612|666x500](upload://2Ujnesf3QK4sBchVD6QryPSUWSL.JPG)
![IMG_0644|666x500](upload://fPHXSvoKisuuIgh7vgmnotuPjGg.JPG)
![IMG_0646|666x500](upload://gNYmw9pcoRYzOGb4V1zQUM6TbbU.JPG)
![IMG_0647|666x500](upload://kx91BVWi3nFCsH65UHezfLPyG6i.JPG)
![IMG_0649|666x500](upload://zCdjcPg1f1BJmQQeWH3JIq0e6WO.JPG)
![IMG_0650|666x500](upload://iepzeunpADze2cm9dgHjdSr4KT3.JPG)
![IMG_0652|666x500](upload://gRiKdpCNHGC6No0ycLwNOJeyXH9.JPG)
![IMG_0645|666x500](upload://5sEqa7KmBXsaIOofwTowAA0uMRr.JPG)

Here are the files:
Schematics:
[https://easyeda.com/Twinsen/NRF_Remote](https://easyeda.com/Twinsen/NRF_Remote)
3D printing files:
[https://www.thingiverse.com/thing:2843488](https://www.thingiverse.com/thing:2843488)
Parts list:
[https://docs.google.com/spreadsheets/d/1Ayte5Xm0up_AQHfdTZghDGnGC5o7WZZo4H4hzZ2LCAw/edit?usp=sharing](https://docs.google.com/spreadsheets/d/1Ayte5Xm0up_AQHfdTZghDGnGC5o7WZZo4H4hzZ2LCAw/edit?usp=sharing)
Code:
[https://github.com/asafteirobert/nRF24-Esk8-Remote](https://github.com/asafteirobert/nRF24-Esk8-Remote)
```

---
## \#2 Posted by: laurnts Posted at: 2018-03-28T20:58:00.805Z Reads: 303

```
Interesting. How much are you selling it for?
```

---
## \#3 Posted by: Twinsen Posted at: 2018-03-28T21:01:39.175Z Reads: 288

```
Something around 50$+shipping from EU. But more on that later since I'm not sure if I will do it at all.

Because I might be looking into redesigning it around the ESP32 to replace both the Arduino Pro mini and NRF module for much better range and more program space.
```

---
## \#4 Posted by: notger Posted at: 2018-04-01T08:29:30.768Z Reads: 263

```
That remote looks exactly like what i'm looking for, cause i do not get along with Thum Control.

Keep us updated if you'd ever sell those remotes or any kind of further developement.
```

---
## \#5 Posted by: Waiboard Posted at: 2018-04-05T22:34:41.100Z Reads: 238

```
Hi, I'm from Argentina and I would like to do the same remote control that you did. In my country, remote controls manufactured for esk8 are not available. But it is easy to get all the components of the list.
I have an electric longboard that uses an ESC X-CAR 120a and I would like to ask you if the remote control works with an ESC?
Also ask yourself if the programming of the Arduino is so simple to connect to the PC and load the code? I have no experience in programming.
Thank you very much!
```

---
## \#6 Posted by: Twinsen Posted at: 2018-04-06T02:35:23.720Z Reads: 218

```
Hello. I use 2 of X CAR Beast ESCs. I designed it for them and it should work with no problem.
For programming the Arduino Pro mini you will need a USB-RS232 adapter but it is quite simple. There are tons of tutorials about it so you should have no problem.
```

---
## \#7 Posted by: Waiboard Posted at: 2018-04-06T02:47:04.503Z Reads: 209

```
[quote="Twinsen, post:1, topic:50482"]
Schematics
[/quote]

Perfect!
If I was investigating a little and I saw that it would not be very difficult.
Another question is how to connect the ESC to the Receiver? (I use 1 ESC only)
I saw in the scheme of the Receiver that they would be pins P1, P2, P3, P4. But I do not understand how to connect it to my ESC that only has 3 wires.
```

---
## \#8 Posted by: Twinsen Posted at: 2018-04-06T11:23:43.668Z Reads: 186

```
P1 and P2 connect to the 3 wire connections on your ESC. P3 is for future use for VESC and P4 us to connect your battery so you can see it's voltage on the remote.

If you have one ESC, connect it to P1 or P2, it doesn't matter. 

One important thing though: If you have 2 ESCs, only one of them should have the 5v connected. Because if you connect both of the power pins together, it might cause problems with their 5v regulators. So one ESC has 3 pins connected, the other only 2.
```

---
## \#9 Posted by: Der6FingerJo Posted at: 2018-04-06T11:36:05.652Z Reads: 174

```
Hey man, nice remote!
Any specific reason to go with the 3,3V Arduino?
```

---
## \#10 Posted by: Twinsen Posted at: 2018-04-06T11:47:08.095Z Reads: 171

```
I use 3V3 Arduino because then I don't need a boost converter. I need 3.3v for the NRF module anyway so I would have to use the larger and more expensive Arduino Nano or a separate 3.3v regulator.

So this way it keeps everything smaller, cheaper and more battery efficient(i should get about 20 hours battery life)

It does have one minor problem that the hall sensor becomes up to 5% less sensitive on very low battery, but I can compensate for it in software if needed.
```

---
## \#11 Posted by: Der6FingerJo Posted at: 2018-04-06T13:00:39.225Z Reads: 174

```
Ah i see. So do you run the nrf off of 4.2V when charged?
```

---
## \#12 Posted by: ElskerShadow Posted at: 2018-04-06T13:05:51.138Z Reads: 169

```
 Very nice remote ! I like the trigger style
```

---
## \#13 Posted by: Twinsen Posted at: 2018-04-07T11:38:33.350Z Reads: 166

```
No, I run the NRF from the regulated 3.3v from the Arduino board regulator
```

---
## \#14 Posted by: FalconNL Posted at: 2018-04-08T20:10:54.392Z Reads: 163

```
This looks great! Can i ask what kind of ESC are you using?
```

---
## \#15 Posted by: Twinsen Posted at: 2018-04-09T01:02:39.452Z Reads: 171

```
I use 2 of these ESCs running on 6s
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html?___store=en_us
with these motors
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5065-320kv-brushless-outrunner-motor.html?___store=en_us

Loads of power. Also the ESCs seem to be great for mountainboards since the throttle level matches a specific RPM. And it also combines nicely with a amperage limit based on throttle.
```

---
## \#16 Posted by: Waiboard Posted at: 2018-04-23T22:40:39.958Z Reads: 161

```
Hello @Twinsen, I finally finished putting together the remote control.
I do not know why the battery icon flashes. The load is 4.3V.

I also do not know why when I turn on the remote control it says "Exit" 50. I think I should dial 0 but it starts at 50.
By pressing the dead man button the engine starts running without having activated the throttle trigger. When he wants to brake, he does not, but he keeps accelerating.
I leave a video that films fast so you can see this and you can help me.
Thank you!

https://youtu.be/OzvGRBi1UGw
```

---
## \#17 Posted by: Twinsen Posted at: 2018-04-23T23:01:21.924Z Reads: 158

```
Nice, you made one. You need to calibrate the hall sensor.
1. Press and hold the Dead man switch while the remote is starting to enter the settings menu.
2. Go to Throttle min, move your stick to the maximum brake position and press the Cruise control button to automatically set the value.
3. Go to Throttle center. Leave your stick to the idle position and press the Cruise control button to automatically set the value.
4. Go to Throttle min, move your stick to the maximum acceleration position and press the Cruise control button to automatically set the value.

If it accelerates when you brake, you need to reverse one of the magnets(the one on top of the sensor when you brake fully)

Output shows 50% when idle, 0%on full brake and 99% on full acceleration.

About the battery, I'm not sure, check your connections. Check the value of "Voltage cal. rem." in the settings menu, it should show the voltage of the battery in parenthesis. I think I calculated for a maximum value of 4.2v. Depending on your resistor tolerances 4.3V might be too much, so try with a 4V battery.
```

---
## \#18 Posted by: Waiboard Posted at: 2018-04-24T02:08:59.542Z Reads: 153

```
Perfect!
I already got the engine to accelerate and brake accordingly, thanks to your comments.
The remote control battery still can not show the correct voltage, so I must have some bad connection. I will corroborate it later.

Thank you very much @Twinsen
```

---
## \#19 Posted by: Twinsen Posted at: 2018-05-19T11:53:36.952Z Reads: 144

```
After a long time I managed to make one in black.

![IMG_1087|666x500](upload://1I8hRa1OtQuptrw7QT1ON62pJ0Y.JPG)
```

---
## \#20 Posted by: Arzamenable Posted at: 2018-06-02T10:46:50.820Z Reads: 136

```
Oh, this exact one is mine! Very cool. I dropped it and broke the OLED after only 24hrs. 😭😭😭😭😭. Cheap enough to get a new one on amazon.
```

---
## \#21 Posted by: Twinsen Posted at: 2018-06-02T14:43:54.164Z Reads: 137

```
Oh that's a real shame. Did you manage to break the oled without breaking the plastic?
I threw mine on the ground a few times when I had minor crashes and had no problems.
```

---
## \#22 Posted by: Arzamenable Posted at: 2018-06-03T03:39:04.799Z Reads: 133

```
I chipped off a small fragment of shell near the screen
```

---
## \#23 Posted by: Arzamenable Posted at: 2018-08-04T23:02:39.197Z Reads: 120

```
![image|500x500](upload://mtysTeBDbc2Z04mHEC9QD7YE2cB.jpeg)

I reshelled it. A very solid remote.
```

---
## \#24 Posted by: Wentworth Posted at: 2018-08-06T08:16:55.713Z Reads: 110

```
What is the software for your waveform acquisition? Can you share it with me?
```

---
## \#25 Posted by: Twinsen Posted at: 2018-08-20T10:01:27.593Z Reads: 94

```
I use a Hantek 6022BE USB oscilloscope connected to a tablet. That's the official Hantek software, not that great really.
```

---
## \#26 Posted by: Wentworth Posted at: 2018-08-21T01:16:05.507Z Reads: 81

```
Thank you.
```

---
## \#27 Posted by: Twinsen Posted at: 2019-04-13T09:49:04.022Z Reads: 54

```
The information here is kind of out of date. New topic here with better information: https://www.electric-skateboard.builders/t/twinsen-s-3d-printed-nrf-remote-v2/91414
```

---
## \#28 Posted by: Qrob Posted at: 2019-08-13T21:09:23.372Z Reads: 13

```
@Twinsen can you make me one for $45 usd
```

---
