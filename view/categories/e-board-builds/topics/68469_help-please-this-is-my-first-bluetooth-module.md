# Help please this is my first Bluetooth module

### Replies: 16 Views: 433

## \#1 Posted by: Blacksheep Posted at: 2018-09-18T23:30:36.970Z Reads: 140

```
I can’t detect with my iPhone my Bluetooth module, can someone help me please ![image|375x500](upload://5jpb5G23NCeDpaem37HyXLL2DLD.jpeg) ![image|375x500](upload://fyyMKY6BSJfnQWZ2OdTDYozxwcg.jpeg) ![image|375x500](upload://xe9wkScZnDFjl3rTamuSvUxw8qK.jpeg) ![image|375x500](upload://BBkd1gUq4leIZ3xdgaw4fPvzVG.jpeg)
```

---
## \#2 Posted by: Blacksheep Posted at: 2018-09-18T23:35:55.945Z Reads: 128

```
![image|375x500](upload://vptgqKrVi3N3mQY71wBwZrnULjz.jpeg)
```

---
## \#3 Posted by: goldrabe Posted at: 2018-09-19T00:07:10.007Z Reads: 123

```
It seems to be a problem with the hm-10 bluetooth clones and android oreo. You have to reflash the original firmware.
@rey8801 has commented on some threads about that.
```

---
## \#4 Posted by: Blacksheep Posted at: 2018-09-19T01:35:36.256Z Reads: 114

```
How do I refresh?
```

---
## \#5 Posted by: goldrabe Posted at: 2018-09-19T02:00:29.425Z Reads: 110

```
@rey8801 is the man to ask, but i guess he is in sweet dreams about his new hubs at the moment (MEZ time zone)  there are also some videos on youtube. Did you tried all the obvious stuff, restarting your phone, fiddling with bluetooth settings ect.?
```

---
## \#6 Posted by: rey8801 Posted at: 2018-09-19T05:07:49.784Z Reads: 97

```
Ahahahah a yes @goldrabe is right :grin: I was dreaming and before that I was working on the hubs! :joy:
You are using an iPhone so you shouldn't have problem of incompatibility. It's only the case with Oreo. Now by the picture I can tell what is different from usualz that depends on the app that you are using and the module. Plus post a Pic of the connection of the HM-10 module.
I see you use 3V, should work as well but I always use 5V. Most of the module accept it. Sometime with 3V is fine to detect the module but then didn't work with me. 
Are you sure about the baud rate? Some app use 9600. We probably use a different one since is iPhone on your case. 
Make sure TX and RX connection are reverse but that should give you problem in receiving and sending data not detect the module. 
Instead of using a vesx related app on your phone try to detect the module with some BLE app from the one available in the Apple store. I use Serial Bluetooth Terminal in Android
Maybe it does exist in IOS too. 
So I would say try to detect it with the other app, if it doesn't work then switch to 5V.if still doesn't work then the module is broken. You can also try with another phone. If the detection doesn't work at all you can try to flash the original for aware. You find instruction on YouTube and Arduino forum but first try with the detection and 5V because usually IOS don't have incompatibility problems.
```

---
## \#7 Posted by: Blacksheep Posted at: 2018-09-19T05:19:11.767Z Reads: 83

```
Ok i will try thanks for all your help o and this is the app ![image|281x499](upload://vjzaHvGKrtFMijNK7svs2WT1kch.jpeg)
```

---
## \#8 Posted by: rey8801 Posted at: 2018-09-19T05:33:03.730Z Reads: 72

```
I checked really fast but seems to me you need 9600 baud rate and not 115200. So try frist that part. Make sure you pres on write in the app on the Vesc tool otherwise you don't really apply the new setting.
```

---
## \#9 Posted by: Blacksheep Posted at: 2018-09-19T05:58:11.179Z Reads: 69

```
Ok thanks so much
```

---
## \#10 Posted by: rojitor Posted at: 2018-09-19T09:50:32.190Z Reads: 68

```
I get this with the escape
![Screenshot_20180919-114607|281x500](upload://8SloNEKspPbULhsbA36jfTfh9bD.png)
```

---
## \#11 Posted by: Acido Posted at: 2019-01-21T18:50:12.835Z Reads: 38

```
Can you help me out?
![Screenshot_4|690x384](upload://rFFPlBKDPioswPIl2LAWODR1m73.png)
```

---
## \#12 Posted by: rey8801 Posted at: 2019-01-21T19:18:39.851Z Reads: 35

```
Sure! Did you solder the Arduino pins  to the module pins? It can work with just the contact but the it works better if you solder them.
```

---
## \#13 Posted by: Acido Posted at: 2019-01-21T19:20:37.109Z Reads: 36

```
I soldered them
![IMG_20190121_201917|281x500](upload://zLZlsfi0BbPKB8MLJa1JMLRxcL5.jpeg) 
Hopefully i soldered the wires on correct pins
```

---
## \#14 Posted by: rey8801 Posted at: 2019-01-21T22:20:34.829Z Reads: 33

```
Pins are correct 7 - 8 - 11. I know it's a stupid question but are you powering the Bluetooth module during the fashing? The esiest is to get 5V and GND from the Arduino uno/nano.
```

---
## \#15 Posted by: Acido Posted at: 2019-01-22T06:01:41.766Z Reads: 31

```
Yes its powered from the nano
The module can be seen in the ackmaniac app but I cant be connected to it, the app chrashes
I can try with another module
```

---
## \#16 Posted by: rey8801 Posted at: 2019-01-22T07:03:36.192Z Reads: 27

```
Of the module can be seen than flashing the module won't help usually. You can test on your phone with the app BLE scanner. If you can connect to it the module is fine. Ackmaniac's app requires all the permission from your phone to work properly and turn on the GPS too. 
Anyhow I found out that tp flash the module when you are sure that the connection are fine I do in this sequence and it works 85% of the time. Open Arduino IDE and connect your Arduino, correct port and module. Load the script. Disconnect the USB from the Arduino. Hm-10 clone module connected with all the 3 pins + 5v and gnd to the Arduino. Then dosconnect the 3 pins on the Arduino nano (keep them in your fingers ready to plug them). Basicaly what you want is load the script on the Arduino and immidiately afterwards send the flashing command to the module. So the sequence is:
Connect the usb (you will see both module and Arduino power on) 
Load the script and wait that is done
Plug the 3 pins inside the Arduino and launch the flashing for the module (better you already prepare the string of code in the terminal windows so that you have to just press ok) 
Try like taht few times, some modules do not work immidiately but they all do at the end (usually 😁). It seems like that the Arduino need to have a fresh code loaded every time. Do not ask me why but for me it works and I have done a lot of modules like that. After thst you should see your module as HM-10 soft on your phone. Anyhow first try BLE scanner of you can connect the module is already fine. Good luck!
```

---
