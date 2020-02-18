# Lake Board &#124; WeFunk DH38 &#124; Caliber II 50 &#124; 10S BMS &#124; APS 6355 190KV &#124; VESC &#124; Arduino

### Replies: 8 Views: 1553

## \#1 Posted by: Pimousse Posted at: 2016-10-17T14:02:57.159Z Reads: 203

```
Hi all,

I started this build in early June and I'm still on it.
It takes time because I'm keeping changing ideas about what I finally want.

So let's go for a quick presentation then I'll try to retrace the history of the build.

## Specs :

- Deck : WeFunk DH38
- Trucks : Caliber II 50° + pads 6mm
- Wheels : ABEC11 Flywheels 83mm 80A
- Bearings : Amphetamine Ceramix silver + speed rings
- Motor mount : DIY ES v4
- Tranmission : 15x36 width 15mm
- Motor : APS 6355 190KV sensored
- Batteries : Flightmax 2x 5S 8000mAh
- BMS : APS BMS 10S + charger
- ESC : DIY ES VESC 4.12
- Enclosure : home made
- Powerswitch : Vedder Powerswitch (esk8.de)
- Remote : GT2B + 3D printed enclosure
- Others : Arduino + LCD2x16 + temperature sensors + switch with led ring, headlight and rearlight

## Features :

- Top speed : 40km/h
- Range : more or less 20km
- Charge smartphones
- Bluetooth music speakers embedded
- LCD screen embedded with tons of infos
- Headlight and rearlight controlled by the remote

## Building the board :

"Christmas everyday" time

<img src="/uploads/db1493/original/3X/5/e/5edddfbe8b096a92ad75b1b4b3cd56a1cbb29731.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/8/08bf11c8dee901f6e8bb088d53eb23a0be88b1db.jpg" width="370" height="499">
<img src="/uploads/db1493/original/3X/f/e/fe711846e9fd02e4cef1ed3c1b12b591fddb6431.jpg" width="675" height="499">

Starting prototyping, making and coding my home made electronic board :

At this point, I wanted to communicate with the VESC though UART, display datas on the LCD, datalog on a microSD card. and control the lights.
The board shall also be a hub to supply power to electronic devices (USB plugs, BT speakers...).
Power supply : UBEC 5A + 2A channel switched by RC receiver using CH3 button of the GT2B.

<img src="/uploads/db1493/original/3X/5/a/5ae523f4432f80e54811b096ff2cee4e22999e3b.jpg" width="666" height="500">

After many hours of coding and modifying the existing Rollinggecko's library (in order to include temperature and fault code management), I finally got a working version of my system.
Almost working I should say, because I was unable to use LCD and microSD board working simultaneously...

https://youtu.be/IEq4MzafLBA

Then I switched to a brand new stuff for me : create the enclosure !
It was not so difficult finally and I'm pretty happy with the result.

<img src="/uploads/db1493/original/3X/8/a/8a6990c56416626f44e62ac9ab03a67253435148.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/a/c/acc02be6db00efed5a34db45c2ae11cbcbc89846.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/8/1/81dc185ee85baf33a126fa580f010b1069ac5cea.jpg" width="666" height="500">

I found with carbon fiber with blue polyester fiber cloth very beautiful !
So I decided to cover the bottom of the board with it.

But before, I painted the edge with the ABEC11 flywheels green color and route the board for the lights wires.
Because the wires are thin, I could put them into a "duct" (actually a bad quality shrink tube I didn't heat) to be able to remove/add/change a wire if needed.

<img src="/uploads/db1493/original/3X/f/2/f2748bfd75e688179e23334631d636095637f3d6.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/0/3/03f8fbc41f6c3c5c69c8d6b09d73e37b71c43a33.jpg" width="668" height="500"><img src="/uploads/db1493/original/3X/7/e/7eda207d7b193b51fe0a6713646f4f5e6960fb50.jpg" width="668" height="500">

After sanding and preparing the routes, time was come to cover the whole board.
Not whole in fact, I wanted to keep clear the hidden surface to avoid blocking RF receiver with a total carbon fiber enclosure.

<img src="/uploads/db1493/original/3X/8/0/80a60bab2494e32bf7582973f95b71bd91df16ae.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/0/6/0684daa9839db8715f1b1e93406fd3fa9988daa1.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/9/5/9580c8a331406125fe527687606c14885c11f063.jpg" width="666" height="500">

Well, it's not Whitepony's quality but anyway... For a first try, it's quite enough for me ! :slight_smile:
And with a epoxy resin layer on it (edge included), if you don't look at it too close, it's clean enough.
 
<img src="/uploads/db1493/original/3X/9/8/98a9cfcb8fc6b42d1676e246f1c2b1d3e37913dd.jpg" width="666" height="500">

That being made, I came back to electronics and build the Mad munkey remote form @FLATLINEcustoms .
Amazing mod after all !

<img src="/uploads/db1493/original/3X/f/a/fa8e056f83e24c78cad304db20026b78df2c1258.jpg" width="374" height="500">

While the 3D printer was still hot, I printed headlight and rearlight enclosure (from scratch).

<img src="/uploads/db1493/original/3X/6/4/64c752bad01a77537db2043b062d53c4f01cc021.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/8/9/89024e4227c550e85577e8044ca6bf887151b397.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/b/6b0583ae4ec860c1244325844fa869513542aa0e.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/6/5/6557fa6e7609371f4076f6f572f1e0df3da032d6.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/e/c/ec277a62c6f57ac076b8db1d18a6b01fd51061e0.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/d/2/d28aa7842471cd0dcfd473bf7867314b6317bfc0.jpg" width="668" height="500">

I published the headlight print on Thingiverse if you're interested in : http://www.thingiverse.com/thing:1813811
I still have a little change to add and it will be in release status.
 
I kept Solidworks open and designed/printed the plug panel (for USB plugs, BMS charger and BT speaker commands)

http://img15.hostingpics.net/pics/987860panelboardv11back.png
(I don't have pictures of the real part, sorry)

At this point, I tested Bluetooth modules (HC05) and played a bit with VESC Monitor.
I fell in love with that !!!
But I had to choose between my own Arduino system and BT because the VESC has only one UART port...
I chose BT.
So I threw my previous board away and started to build a new one with these small features :
- Measure battery voltage (with a voltage divider) and display it
- Measure temperature inside the enclosure
- Still support a hub connection with now 2 different supplies : main and switched for light control.
 
<img src="/uploads/db1493/original/3X/9/9/9988dec6d736047d33ff2ab57b0aa53d7f1863ec.jpg" width="666" height="500">

Time was come to put all these stuff on the board and screw the enclosure.

But I missed some point during the build and the enclosure was too small to fit with the implementation of the elements.
Basically, the only way to close the box is to put the powerswitch above the BMS.

<img src="/uploads/db1493/original/3X/3/d/3dd8c3a118134caa25b8bffa97a46d1327e93f75.jpg" width="666" height="500">

So I designed and printed a structure to make it possible without electrical and thermal issues.
I had to modify it because the switches on the enclosure are hitting it...
Here is what the build looks like presently :

<img src="/uploads/db1493/original/3X/b/3/b300bf9d10f7ce8dd3e7df63d6d78007efaf8768.jpg" width="374" height="500">

Yesterday I decided to drill and set the insert for screwing the enclosure.
I was still a bit "tired" of the party and didn't make a good job...

I cut the headlight wires (I drilled in it, I forgot it was behind :sweat_smile: ), the powerswitch doesn't want to switch off anymore and one of the LED of the rearlight is fried.
Time to sleep I guess. :relieved:

## To do :

- Replace the headlight wire
- Replace the powerswitch (the new one is on the road, thousand thanks to @elkick )
- Adjust components to close easily and safely the enclosure
- Some wire length adjustment
- RIDE, RIDE, RIDE and RIDE !!!! :grinning:
```

---
## \#2 Posted by: sismeiro Posted at: 2016-10-18T10:43:01.343Z Reads: 153

```
Hi, your project it's looking good. Keep us posted. :slight_smile:
```

---
## \#3 Posted by: SteveS Posted at: 2016-10-18T15:02:00.612Z Reads: 141

```
Very nice design ideas. Look forward to more posts!
```

---
## \#4 Posted by: jmasta Posted at: 2016-10-19T01:16:46.481Z Reads: 130

```
This is really great!  I like your 16x2 Arduino display

If you had two Bluetooth module modules - one directly connected to UART  and another connected to your Arduino - wouldn't you be able to use it simultaneously with the VESC Monitor app on your phone?  My understanding of Bluetooth is that it is analogous to a message board... as in,  one source can post data which can then be read by multiple devices.  I think it's possible to have the best of both worlds here. Your Arduino system + smart phone bluetooth app
```

---
## \#5 Posted by: Jebe Posted at: 2016-10-19T06:05:24.715Z Reads: 111

```
Love that blue carbon
```

---
## \#6 Posted by: Pimousse Posted at: 2016-10-19T06:29:55.914Z Reads: 109

```
@jmasta : That's not possible, because BT doesn't work so simply. It's a master/slave communication.
The VESC doesn't give any datas as long as you don't ask him for it.
So it works like this :
Master (Smartphone) : "Hello, give me data. Stop"
Slave (VESC) : "Here there are : xxxxyyyyzzzz. Checkcode. Stop"

And between both Smartphone and VESC devices, BT modules handle the communication with some handshaking or so to be sure to communicate with the right partner.

It's my understanding and tried to keep the explanation simple but I could be wrong as well :blush: 

@sismeiro, @SteveS, @Jebe Thanks guys ! :slight_smile:
```

---
## \#7 Posted by: smurf Posted at: 2016-10-19T07:41:39.753Z Reads: 103

```
You can passively capture data exchanges between two BLE devices, pushing the data into Wireshark, the open source network analysis tool, 

https://www.adafruit.com/products/2269
```

---
## \#8 Posted by: Pimousse Posted at: 2016-10-19T09:26:17.639Z Reads: 101

```
It's quite an interesting tool !
However, I don't use BLE (I chosen HC05 for v2.0 + EDR BT because BLE has a lower range especially in a carbon enclosure configuration) and my skills seem too limited to implement a sniffer on my Arduino.
I don't think it's worth it.

Anyway, I keep in a corner. :wink:
```

---
