# Wiiceiver Controller

### Replies: 38 Views: 5096

## \#1 Posted by: andrewhannay Posted at: 2016-05-10T08:49:12.615Z Reads: 295

```
Does anyone know if you can still get hold of these kits.
The last post on austindavid.com seems to be August 2015.
Is there an alternative controller with the same sort of features as the Wiiceiver.
I have a lttle Arduino board and wireless Nunchuck that I am about the experiment with, but was just making sure that the controller thing hasn't moved on to something else.
Andrew
```

---
## \#2 Posted by: lox897 Posted at: 2016-05-10T10:10:20.267Z Reads: 292

```
You can buy it assembled from @torqueboards . They have a lot of drop out issues though. I would go with 2.4ghz.
```

---
## \#3 Posted by: andrewhannay Posted at: 2016-05-10T14:05:43.043Z Reads: 273

```
Drop outs? That's not good, I presume something to do with cheap wiimotes?
When you say go 2.4ghz are you talking about standard rc car controllers? I find them rather bulky and would rather something hand held (Palm size)
Andrew
```

---
## \#4 Posted by: delta_19 Posted at: 2016-05-10T15:50:38.462Z Reads: 263

```
all wiimotes have a lot of drop-outs so its not really that cheap ones are being used.

and for 2.4 Ghz you could get TB's mini 2.4 product/torqueboards-2-4ghz-mini-remote-controller/
```

---
## \#5 Posted by: JLabs Posted at: 2016-05-10T17:20:49.486Z Reads: 242

```
Austin David and torqueboards no longer sell them, I have had no issues witht the drop outs. My controller works just fine except yesterday when I had to replace the atmega, there are no other controllers with throttle smoothing and cruise control which is why I use it
```

---
## \#6 Posted by: willpark16 Posted at: 2016-05-11T00:22:41.918Z Reads: 225

```
dropouts occur due to signal loss so if you intend to be going under a lot of bridges, very fast, or in an area where there isnt a good cell phone signal then dont buy bluetooth.
```

---
## \#7 Posted by: Bender Posted at: 2016-05-11T05:09:22.470Z Reads: 211

```
[quote="willpark16, post:6, topic:3057, full:true"]
dropouts occur due to signal loss so if you intend to be going under a lot of bridges, very fast, or in an area where there isnt a good cell phone signal then dont buy bluetooth.
[/quote]

Your joking right?!?
```

---
## \#8 Posted by: willpark16 Posted at: 2016-05-11T05:11:01.761Z Reads: 200

```
Huh now im a bit confused
```

---
## \#9 Posted by: Bender Posted at: 2016-05-11T05:13:27.046Z Reads: 197

```
Blutooth has nothing to do with cell towers
```

---
## \#10 Posted by: willpark16 Posted at: 2016-05-11T05:14:42.913Z Reads: 189

```
no u misunderstood i wasnt talking about cell towers im taking about areas with lots of mountains and basically anywhere else u can lose a signal.
```

---
## \#11 Posted by: willpark16 Posted at: 2016-05-11T05:15:47.029Z Reads: 180

```
elevation actually is an issue because I live quite high up and had issues with bluetooth
```

---
## \#12 Posted by: Bender Posted at: 2016-05-11T05:20:49.603Z Reads: 185

```
Again that has nothing to do with bluetooth
Do your blutooth headphones cut out in the mountains? No.

It's been determined that the dropouts are do to not soldering to directly or the board or from interference from the reciever being too close to the motor wires.
There are quite a few people that have never had dropouts, including me, if it set up correctly
```

---
## \#13 Posted by: lowGuido Posted at: 2016-05-11T05:21:58.577Z Reads: 188

```
I have built 7 or 8 boards all using nyko kama nunchucks and when soldered on properly never had droppouts. Its generally caused by poor connection of the receiver dongle.
```

---
## \#14 Posted by: willpark16 Posted at: 2016-05-11T05:22:42.145Z Reads: 178

```
uguys are lucky bastards then because up here none of my bluetooth devices work while im on the move
```

---
## \#15 Posted by: Bender Posted at: 2016-05-11T05:25:09.115Z Reads: 183

```
Bummer, that's news to me
That's not the way blutooth works but obviously something is going on.
Other wireless devices that operate in the 2.4 GHz or 5 GHz bandwidth (microwave transmitters, wireless cameras, baby monitors, a neighbor's Wi-Fi device) can cause interference with bluetooth connections.
```

---
## \#16 Posted by: andrewhannay Posted at: 2016-05-11T08:57:50.924Z Reads: 183

```
That all went off at a bit of a tangent.
Yes, Bluetooth is point to point so no worry of interference from bridges or mountains, I think willpark16 is confusing loss of signal on his phone when using bluetooth headset or a car handsfree.
Ok, so dropouts could be caused by interference from motor and/or bad connection to Wiimote receiver. I notice that in the circuits I have found no one uses pull up resistors which should normally be fitted when using I2S-like serial comms. More and more people develop embedded software projects on the hobbie-type prebuilt ATmega or Arduino platforms and just pull in pre-written libraries without considering how the hardware should be set up in a real world.
I will persevere with a Wiimote setup and, if I have time at work :-), will look at the signals on an oscilloscope.
```

---
## \#17 Posted by: Bender Posted at: 2016-05-11T11:06:41.372Z Reads: 173

```
[quote="andrewhannay, post:16, topic:3057"]
I will persevere with a Wiimote setup and, if I have time at work :-), will look at the signals on an oscilloscope.
[/quote]

Sweet!

Also on lowGuidos advise I installed a ferite ring between the reciever and VESC
```

---
## \#18 Posted by: willpark16 Posted at: 2016-05-16T06:48:30.088Z Reads: 169

```
actually no im not. Bluetooth and Wi-Fi have shared the same 2.4GHz frequency spectrum for a long time, which can cause the radio signals to interfere with each other. This is especially noticeable when you are on a phone call using your Bluetooth headset in your office or in your house, and you hear static. Quite often, the solution may be to turn off Wi-Fi on your phone while you are talking using Bluetooth. However, if you cannot turn off Wi-Fi, then move closer to the Wi-Fi access point. This may make the Wi-Fi connection more robust, which will make it easier for the phone to time-share the radio spectrum between Bluetooth and Wi-Fi traffic.
```

---
## \#19 Posted by: andrewhannay Posted at: 2016-05-16T08:40:03.646Z Reads: 168

```
Ok, I see what your saying now. so interference can come from Wifi which occupies quite large bands of the 2.4GHz spectrum causing the BT to hop or search for another side band possibly causing complete loss of signal. Maybe you have lots of interfering Wifi signals near by. Or maybe other RC handsets?
Thanks for clearing that up anyway.
```

---
## \#20 Posted by: andrewhannay Posted at: 2016-05-16T08:45:57.554Z Reads: 168

```
I have noticed that some skateboard controllers especially the early ones have a copper or some sort of conductive band on the outside of the controller. I suspect this is the transmitter output carried to the outside of the handset onto your hand that then uses your body as an antenna, carrying the signal all the way to your foot which is really close to the receiver. This allows the handset to transmit at a very low power saving battery life and at the same time including a security feature that stops the board from being operated if you are not standing on directly on it. I wonder if I can do that with the Wiimote controller to prevent signal loss.
```

---
## \#21 Posted by: lowGuido Posted at: 2016-05-16T10:45:38.702Z Reads: 153

```
I dont think you even need it. I can connect my nunchuck to my board from 6 meters away. And im never that far from it.
```

---
## \#22 Posted by: andrewhannay Posted at: 2016-05-25T09:39:22.319Z Reads: 157

```
Ok, update. I've built my own Wiiceiver.
I bought some really cheap Wireless nunchucks from eBay. When I say cheap, I mean cheap - 2 sets for less than £7, unfortunately they are pink!
I also bought some really small Arduino Pro mini boards. So small in fact they could fit inside a nunchuck receiver.......which got me thinking. :slight_smile:
I had problems getting the nunchucks to connect due to them insisting on using 400khz serial bus connection which is quite tricky to do using the standard (almost amateur) Arduino libraries but I found a way. I also had to modify the main code as the nunchucks would never connect reliably or quickly. But I think I've cracked it. Check out the pics. 

<img src="/uploads/db1493/original/2X/c/cca9e62792933325ab0a31247af948877cf0b3a0.jpeg" width="375" height="500">

<img src="/uploads/db1493/original/2X/a/a1549fc54c0813d05ccecc5af08d779033c5c285.jpeg" width="666" height="500">
 
<img src="/uploads/db1493/original/2X/1/15011d97dad0544e3bd6d7ab13ce8965fc03b924.jpeg" width="666" height="500">

<img src="/uploads/db1493/original/2X/7/73f92676e655e23ecef0f2bb08da5e735c358c83.jpeg" width="666" height="500">
```

---
## \#23 Posted by: Maxid Posted at: 2016-05-25T09:50:18.731Z Reads: 143

```
nice - can you show the code as well? No modification to the handset necessary? If this is in fact that easy I will do the same thing - getting a nyko kama in Europe is not easy :slight_smile:
```

---
## \#24 Posted by: JLabs Posted at: 2016-05-25T11:12:31.853Z Reads: 141

```
Looks awesome! More details!!
```

---
## \#25 Posted by: lowGuido Posted at: 2016-05-25T11:30:25.795Z Reads: 146

```
yeah more deets!
does it have perpetual steez?
```

---
## \#26 Posted by: andrewhannay Posted at: 2016-05-25T15:03:02.008Z Reads: 141

```
I haven't tested it yet. I need to make sure it's ok before I release code.
It's based on the original Austin David code with a few dodgy mods.
100khz comms changed to 400khz by adding one extra line.
I shortened the wait time to 100ms when scanning for the nunchuck and now it continuously scans until it finds it.
I found the code would hang on waiting for zero after connecting, so I just remove that bit of code :slight_smile:
I guess I need no inform Austin of any changes or upload it to the github?
Andrew
```

---
## \#27 Posted by: Okami Posted at: 2016-06-03T11:09:32.119Z Reads: 130

```
Cool. Give more info when you can.. I would also be very interested in this sort of thing..
```

---
## \#28 Posted by: andrewhannay Posted at: 2016-06-03T12:28:29.600Z Reads: 130

```
Ok, so I've tested it and it seems to work great. :slight_smile:
I bought another cheap Wii Wireless Nunchuck from ebay that isn't pink and that also works without any more mods to the software.
I guess I should upload it back to the software repository so others can view it and download it, but in the meantime can I just add it as a zip to this thread?
Andrew
```

---
## \#29 Posted by: lowGuido Posted at: 2016-06-03T13:14:55.244Z Reads: 130

```
that is excellent news!
I don't know that this forum can accept zip files. but i do encourage you to share the link when you do have it uploaded somewhere.
```

---
## \#30 Posted by: andrewhannay Posted at: 2016-06-14T22:08:57.720Z Reads: 127

```
I've sent the code to Austin to look at however I have found a wireless nunchuck in eBay that works without any software mods. See my next post :-)
```

---
## \#31 Posted by: andrewhannay Posted at: 2016-06-14T22:10:35.245Z Reads: 141

```
Hi all,
This Wireless nunchuck works with the wiiceiver code without any mods. It's cheap and very stylish compared to the pink ones I got. 

https://www.ebay.co.uk/itm/331847694924 

Andrew
```

---
## \#32 Posted by: abaddon6w Posted at: 2016-09-19T05:32:11.617Z Reads: 119

```
Hey everyone. My current build is a 149kv turnigy motor / 6S LIPO / HOBBYWING MAX8 150A / Arduino UNO / Nyko Kama Wiiciever. I am 183 pounds. The wiiciever signal seems to drop and reset the esc occasionally as I'm cruising around. I believe it happens at a higher frequency when I am going full speed. I have turned off low voltage cutoff on the ESC. I'm not sure if this is a wiiciever related issue or just that my board is pulling too much amperage at full throttle under load. This only occurs under load. Any help would be much appreciated.
```

---
## \#33 Posted by: Bender Posted at: 2016-09-19T08:39:32.069Z Reads: 119

```
Do you have a ferrite ring installed?
Have you tried  moving the location of the wiiceiver? Too close to power or phase wires can cause interference, higher speed=higher amp draw. Also make sure all connections are soldered, higher speed=more vibrations.
It is hard to see when riding but if the wii remote disconnects the red light on the nunchuck flashes for a few seconds, might be able to help you figure out if it's the esc or the remote.
```

---
## \#34 Posted by: abaddon6w Posted at: 2016-09-19T16:47:08.040Z Reads: 113

```
I do not have a ferrite ring installed. Where should I install it? 

I also have not moved the location of the wiiceiver. I'll try this and update the post. 

The wiimote does start blinking, but I'm still not sure if it is blinking because the system has lost power or because the signal was lost. I guess if the system lost power and restarted itself then the wiimote would shut off completely?
```

---
## \#35 Posted by: 3dman Posted at: 2017-11-30T14:12:05.721Z Reads: 48

```
@andrewhannay

The controller you mention in the post just above, will connect to the vesc as the Nyco nunchuck? 

Thanks
```

---
## \#36 Posted by: andrewhannay Posted at: 2017-11-30T23:16:51.244Z Reads: 43

```
You will need the Wiiceiver board.
```

---
## \#37 Posted by: 3dman Posted at: 2017-12-01T07:40:12.181Z Reads: 42

```
@andrewhannay. Thanks for the reply. I have a VESC and e what I understand is tat it has that feature built in? So I might not need Wiiceiver.
```

---
## \#38 Posted by: andrewhannay Posted at: 2017-12-01T13:20:00.802Z Reads: 34

```
Oh, I see. I didn't realise the VESC had it built in. In that case it that Wii-mote above was more compatible than the pink thing I had. It wasn't too expensive so worth buying and trying out.
```

---
