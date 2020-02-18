# Sparkswitch + UART and nrf modules on 1 pcb (Arduino Compatible)

### Replies: 62 Views: 5858

## \#1 Posted by: Sander Posted at: 2016-12-13T17:32:38.798Z Reads: 256

```
Hey guys!
I'm making a circuit with ATMEGA328P-AU as the "processor" with the Arduino bootloader.
It will be embedded with Vedders Anti Spark, NRF24L01(2.4ghz transciever), HM-10(4.0 bluetooth for IOS & Android), and UART for the VESC. I will create tutorials of making apps for iOS, programming the board etc.
I will make it open source when I'm done.

Circuit Front:
<img src="/uploads/db1493/original/3X/7/6/76ff2a92c656df9e018368461474fa05dd57fd59.png" width="436" height="500">
Circuit Back:
<img src="/uploads/db1493/original/3X/7/0/702d320f9ebe6df8b8c5d0b74450b35889529751.png" width="436" height="500">

Keep in mind these are not the final circuits. It will change because everything isnt correct. More will be added of requests.

It will have a weak mid spot so you can just break the pcb in two if you dont wan't the vedder's switch on the same pcb: <img src="/uploads/db1493/original/3X/0/7/07247501ab402dd134bb013b48313f444f861d9b.jpg" width="690" height="388">

This circuit was designed for me in the beginning. :stuck_out_tongue: 

Feel free to leave suggestions etc.
```

---
## \#2 Posted by: rpn314 Posted at: 2016-12-13T17:39:47.551Z Reads: 228

```
[quote="Sander, post:1, topic:14608"]
Hey I am wondering how much volt the PPM gives out?
[/quote]

I'm not following what you're asking for entirely. The PPM is usually an input...but the middle pin is 5V. Is that what you needed?
```

---
## \#3 Posted by: Sander Posted at: 2016-12-13T17:42:05.565Z Reads: 224

```
[quote="rpn314, post:2, topic:14608"]
I'm not following what you're asking for entirely. The PPM is usually an input...but the middle pin is 5V. Is that what you needed?
[/quote]


Yes I am asking for that pin in the middle. Is it reliable?
```

---
## \#4 Posted by: Maxid Posted at: 2016-12-13T17:45:44.354Z Reads: 213

```
there are 5V output pins on the VESC - why not use those?
```

---
## \#5 Posted by: rpn314 Posted at: 2016-12-13T17:45:53.455Z Reads: 199

```
Oh, I somehow thought you had the inner pin circled. My eyes are going apparently :worried:

As to it's reliability, I've never heard of any issues. I doubt it can drive much current though. What's your application?
```

---
## \#6 Posted by: Sander Posted at: 2016-12-13T17:53:16.536Z Reads: 206

```
[quote="Maxid, post:4, topic:14608, full:true"]
there are 5V output pins on the VESC - why not use those?
[/quote]

lol, I suck at asking, I meant is it reliable and how much voltage? Also I know now its reliable and it gives out 5V.

[quote="rpn314, post:5, topic:14608"]
Oh, I somehow thought you had the inner pin circled. My eyes are going apparently :worried:

As to it's reliability, I've never heard of any issues. I doubt it can drive much current though. What's your application?
[/quote]

Im gonna run a chip and some lights. I am already doing it on my old e-board with no problem.
Its a circuit with inbuilt 2.4 ghz for remote, and 4.0 bluetooth for my phone.

This is the circuit Im gonna use for my new eboard with inbuild vedder switch that I just made now:
<img src="/uploads/db1493/original/3X/0/b/0b486a9c27dfa030ea8176bc931d7347bcb7b8d8.jpg" width="690" height="388">
```

---
## \#7 Posted by: Maxid Posted at: 2016-12-13T17:55:38.018Z Reads: 188

```
[quote="Sander, post:6, topic:14608, full:true"]
lol, I suck at asking, I meant is it reliable and how much voltage? Also I know now its reliable and it gives out 5V.
[/quote]

What I meant was that when all you need are 5V you should use one of the discrete 5V pins on the VESC and not the receiver pins.
```

---
## \#8 Posted by: Sander Posted at: 2016-12-13T18:09:50.309Z Reads: 180

```
[quote="Maxid, post:7, topic:14608"]
What I meant was that when all you need are 5V you should use one of the discrete 5V pins on the VESC and not the receiver pins.
[/quote]

Oh that one smart idea... I forgot about that one
```

---
## \#9 Posted by: rpn314 Posted at: 2016-12-13T18:11:50.410Z Reads: 179

```

[quote="Maxid, post:7, topic:14608"]
What I meant was that when all you need are 5V you should use one of the discrete 5V pins on the VESC and not the receiver pins.
[/quote]


I'm pretty sure all of the 5V pins are connected to the same circuit so it really wouldn't matter.[quote="Sander, post:6, topic:14608"]
Im gonna run a chip and some lights. I am already doing it on my old e-board with no problem.Its a circuit with inbuilt 2.4 ghz for remote, and 4.0 bluetooth for my phone.
[/quote]
Interesting. So two completely unrelated circuits on the same board? I assume the 5v has nothing to do with the vedder-ish switch?
```

---
## \#10 Posted by: Sander Posted at: 2016-12-13T18:41:22.596Z Reads: 160

```
[quote="rpn314, post:9, topic:14608"]
Interesting. So two completely unrelated circuits on the same board? I assume the 5v has nothing to do with the vedder-ish switch?
[/quote]

Haha you are right. That switch tolerate 60V and 240Amp. But my circuit needs 5 volt to operate. And the bluetooth and 2.4ghz transciever needs 3.3v. So I have a voltage regulator that works from 4.5 -> 7 volt that makes it down to 3.3v. The chip that I program on it works only from 1.8 -> 5.5 Volts
```

---
## \#11 Posted by: lox897 Posted at: 2016-12-13T20:46:32.530Z Reads: 154

```
[quote="Sander, post:6, topic:14608"]
Im gonna run a chip and some lights. I am already doing it on my old e-board with no problem.Its a circuit with inbuilt 2.4 ghz for remote, and 4.0 bluetooth for my phone.

This is the circuit Im gonna use for my new eboard with inbuild vedder switch that I just made now:
[/quote]
Sounds epic! Are you going to open source it once finished?
```

---
## \#12 Posted by: Sander Posted at: 2016-12-13T20:53:01.060Z Reads: 150

```
[quote="lox897, post:11, topic:14608"]
Sounds epic! Are you going to open source it once finished?
[/quote]



Of course! OPEN SOURCE IS LIFE!! I hope its okay I use Vedder's Antispark? But I will give him credit and link for it tho. :blush:

And I will make a tutorial  about how to make an app for your e-board :wink:
```

---
## \#13 Posted by: lox897 Posted at: 2016-12-13T20:54:14.830Z Reads: 145

```
Pretty sure the rule is that as long as you share you can do any imrpovements you want. So are you pretty much combining a hm10 and sparkswitch onto one board?
```

---
## \#14 Posted by: Sander Posted at: 2016-12-13T20:55:15.496Z Reads: 145

```
Yes, I am combinding, an atmega328p-au controller that you can program. An nrf24l01 transciever and hm-10 bluetooth.
```

---
## \#15 Posted by: lox897 Posted at: 2016-12-13T20:56:14.186Z Reads: 155

```
This might be of use to you:

https://github.com/Ladvien/HM-10
https://github.com/Keeward/HM-10
```

---
## \#16 Posted by: Sander Posted at: 2016-12-13T21:06:31.277Z Reads: 159

```
[quote="lox897, post:15, topic:14608, full:true"]
This might be of use to you:

https://github.com/Ladvien/HM-10https://github.com/Keeward/HM-10
[/quote]

Awesome! But I think I might have connected it right...

<img src="/uploads/db1493/original/3X/6/f/6f855e869b5203fef8d31c345ad0a40c786b5848.jpg" width="690" height="388">

Circuit Size(39.93x51.46mm)
```

---
## \#17 Posted by: Sander Posted at: 2016-12-13T21:10:03.500Z Reads: 156

```
[quote="lox897, post:15, topic:14608, full:true"]
This might be of use to you:

https://github.com/Ladvien/HM-10https://github.com/Keeward/HM-10
[/quote]

Im not sure if I connected the bluetooth right...
I connected the UartRx and UartTx to the pin D8 & D9(Arduino Pin).
And to the regulator 3.3v. And I connected all to grounds.
```

---
## \#18 Posted by: lox897 Posted at: 2016-12-13T21:23:29.631Z Reads: 158

```
This is the ATMEGA328P-AU you are using right? <img src="/uploads/db1493/original/3X/7/f/7fd40255d1a451db2c8a328cede6a179b20a292f.PNG" width="500" height="500">
```

---
## \#19 Posted by: lox897 Posted at: 2016-12-13T21:26:45.035Z Reads: 154

```
I would use PD6 as RX and PD7 as TX. Remember that HM10 TX goes to ATMEGA RX and HM10 RX goes to ATMEGA TX. Then use 3.3v VCC or 5v VCC depending on if the module has a voltage regulator or not and then GND to GND.
```

---
## \#20 Posted by: lox897 Posted at: 2016-12-13T21:28:07.183Z Reads: 154

```
You might as well use the 5v or 3.3v and gnd off the uart pins on the vesc, since that is where the rx and tx will come from.
```

---
## \#21 Posted by: Sander Posted at: 2016-12-13T21:36:16.013Z Reads: 152

```
[quote="lox897, post:19, topic:14608, full:true"]
I would use PD6 as RX and PD7 as TX. Remember that HM10 TX goes to ATMEGA RX and HM10 RX goes to ATMEGA TX. Then use 3.3v VCC or 5v VCC depending on if the module has a voltage regulator or not and then GND to GND.
[/quote]

"Remember that HM10 TX goes to ATMEGA RX and HM10 RX goes to ATMEGA TX" Not always. If you use SoftwareSerial you can have it on which ever pin you want. And the ATMEGA TX and RX I use for the VESC data. So you can get voltage, ampere etc. But I havent made a path of it in the circuit yet. Thanks for reminding me :wink: 

Here is an example of using SoftwareSerial(Its how I use the HM-10 Bluetooth):

include "SoftwareSerial.h"
include "SPI.h"
SoftwareSerial mySerial(7, 8);

void setup(){
mySerial.begin(9600);
}

void bluetooth() {

  while (mySerial.available()) {
    char c = mySerial.read();

    textString += c;

    if (textString == "CLR:")
    {
      bColor = true;
      textString = "";
    }

    if (bColor == true)
    {
      //Serial.print(textString);
      if (textString == "CR") {
        cRed = true;
        textString = "";
      }

      if (textString == "CB") {
        cBlue = true;
        textString = "";
      }

      if (textString == "CG") {
        cGreen = true;
        textString = "";
      }

      if (cRed) {
        if (c == ',') {
          int txtstringLength = textString.length();
          textString.remove(txtstringLength - 1);
          red = textString.toInt();
          textString = "";
          cRed = false;
        }
      }

      if (cGreen) {
        if (c == ',') {
          int txtstringLength = textString.length();
          textString.remove(txtstringLength - 1);
          green = textString.toInt();
          textString = "";
          cGreen = false;
        }
      }

      if (cBlue) {
        if (c == ',') {
          int txtstringLength = textString.length();
          textString.remove(txtstringLength - 1);
          blue = textString.toInt();
          textString = "";
          allPixels(red, green, blue);
          if (bLights) {
            pixels.show();
          }
          cBlue = false;
        }
      }
    }

    if (c == '.') {
      bColor = false;
      //Serial.println(textString);
      recievedMessage(textString);
      textString = "";
    }
  }
  lightMode(lMode);
}
```

---
## \#22 Posted by: lox897 Posted at: 2016-12-13T21:38:17.278Z Reads: 122

```
But that is for softwareserial. The vesc needs it that way.
```

---
## \#23 Posted by: Sander Posted at: 2016-12-13T21:39:15.228Z Reads: 122

```
[quote="lox897, post:22, topic:14608, full:true"]
But that is for softwareserial. The vesc needs it that way.
[/quote]

No, the VESC is using the Serial also the TX and RX is the Serial.
```

---
## \#24 Posted by: lox897 Posted at: 2016-12-13T21:40:41.668Z Reads: 121

```
Oh ok. Whatever you think... I would wire rx to tx and tx to rx since that is what everyone does.
```

---
## \#25 Posted by: Sander Posted at: 2016-12-13T21:45:23.375Z Reads: 125

```
[quote="lox897, post:24, topic:14608, full:true"]
Oh ok. Whatever you think... I would wire rx to tx and tx to rx since that is what everyone does.
[/quote]

I think you are misunderstanding me or I am not clear. 

There is a library called SoftwareSerial for the ATMEGA. It allows you to connect and communitcate with multiple communication ports. So you set it up with ex. mySerial(tx, rx);. You can choose whatever pin you want! The UART of the VESC only works with the SERIAL that is pin 0 and 1! Because of the way that code is written. I will probably rewrite it because I like to have the Serial in not use so you can debug. with the Serial Monitor.

So you are talking about the VESC? Im talking about the bluetooth.

With the VESC its RX and TX on ATMEGA because of the way its written. But I would much more prefer SoftwareSerial so its easier to see whats happening. And fixing bugs.
```

---
## \#26 Posted by: lox897 Posted at: 2016-12-13T21:48:13.187Z Reads: 120

```
I have no idea of what you are saying. Please send a picture of yourschematic of your pcb to me via PM so I can look at it and understand what you mean. I am talking about the wiring from atmega to hm10 and if I look at your schematic I can confirm what I mean.
```

---
## \#27 Posted by: Sander Posted at: 2016-12-13T21:48:50.165Z Reads: 132

```
[quote="lox897, post:26, topic:14608, full:true"]
I have no idea of what you are saying. Please send a picture of yourschematic of your pcb to me via PM so I can look at it and understand what you mean. I am talking about the wiring from atmega to hm10 and if I look at your schematic I can confirm what I mean.
[/quote]

I have no schematics... But I can create one now.
```

---
## \#28 Posted by: Sander Posted at: 2016-12-13T21:54:49.207Z Reads: 133

```
<img src="/uploads/db1493/original/3X/c/1/c175f13b47db13c6b5a1978dd18920a96018abc7.jpg" width="690" height="388">
And it get the power from the UART too because its 3 volt there and 5v. So I dont really need to have a 3v3 regulator
```

---
## \#29 Posted by: saul Posted at: 2016-12-13T22:05:52.094Z Reads: 128

```
hey this is really cool! I just finished soldering a couple nano + nrf with pins for lights and whatever and it was a pain! takes for ever to get all the connections.

I'm not sure it makes any sense to put the spark switch on the same board tho. that thing will have lots of current going through it, if something fries the rest of the circuit is kinda lost too.....

blue tooth is nice, but maybe add a cuttoff switch? it can be hacked if someone really wanted too. not fun!
```

---
## \#30 Posted by: Sander Posted at: 2016-12-13T22:08:30.321Z Reads: 123

```
[quote="saul, post:29, topic:14608, full:true"]
hey this is really cool! I just finished soldering a couple nano + nrf with pins for lights and whatever and it was a pain! takes for ever to get all the connections.

I'm not sure it makes any sense to put the spark switch on the same board tho. that thing will have lots of current going through it, if something fries the rest of the circuit is kinda lost too.....

blue tooth is nice, but maybe add a cuttoff switch? it can be hacked if someone really wanted too. not fun!
[/quote]

You are right. But I don't think the sparkswitch wont be a problem. But I was creating this for my board, but then people suddenly got interested :3 So I am making it public. Yes I can add a switch you can turn the power of the bluetooth.

And to point it out the bluetooth has passwor.
```

---
## \#31 Posted by: saul Posted at: 2016-12-13T22:13:55.570Z Reads: 120

```
well there have been a few reports of spark switches going bust recently. I just think the wireless module on its own would be much better. I want a few of those if you cut the pcb in half. or maybe i'll finally learn eaglecad!

oh and passwords can be broken in a few minutes now...
```

---
## \#32 Posted by: Sander Posted at: 2016-12-13T22:17:51.148Z Reads: 128

```
[quote="saul, post:31, topic:14608, full:true"]
well there have been a few reports of spark switches going bust recently. I just think the wireless module on its own would be much better. I want a few of those if you cut the pcb in half. or maybe i'll finally learn eaglecad!

oh and passwords can be broken in a few minutes now...
[/quote]

Yeah, the bluetooth password can be broken easily btw Im using Circuit Maker http://circuitmaker.com/
the Eagle Cad is probably better ;)

About the wireless, you will need another NRF24L01 with an Arduino bootloader that is running it with the same setup with the package sending.
```

---
## \#33 Posted by: saul Posted at: 2016-12-13T22:27:52.182Z Reads: 125

```
Yea i'm using a couple of these for tx/rx but no bt since i'm just controlling with ppm for now. I can use the regular serial pins on the vesc for bt separately.

Still working on the code, i'm going to open source it soon, but that hardware would save me time for the next ones.

<img src="/uploads/db1493/original/3X/a/0/a0dc8dcdef69107e736d53236b1000b6ca3eb078.jpg" width="690" height="387">
```

---
## \#34 Posted by: Sander Posted at: 2016-12-13T22:37:10.471Z Reads: 120

```
[quote="saul, post:33, topic:14608"]
Yea i'm using a couple of these for tx/rx but no bt since i'm just controlling with ppm for now. I can use the regular serial pins on the vesc for bt separately.

Still working on the code, i'm going to open source it soon, but that hardware would save me time for the next ones.
[/quote]

Awesome controller! I can provide you with my hardware if it will help xD
```

---
## \#35 Posted by: Sander Posted at: 2016-12-13T22:39:38.225Z Reads: 126

```
[quote="saul, post:31, topic:14608, full:true"]
well there have been a few reports of spark switches going bust recently. I just think the wireless module on its own would be much better. I want a few of those if you cut the pcb in half. or maybe i'll finally learn eaglecad!

oh and passwords can be broken in a few minutes now...
[/quote]

I added where you can add a switch that turns the power of the HM-10 on and off, beside the "T R" for TX and RX of the ATMEGA. That is where you connect to the VESC for data. the + L - is for neopixel lights. - + P is the ground input 5v input and the pulse output for controlling the speed of the vesc.

<img src="/uploads/db1493/original/3X/7/9/792fdeda7ed39a05ca91ed330b0f49127e83c80b.jpg" width="690" height="388">

<img src="/uploads/db1493/original/3X/f/9/f950c51142eb6a9282e54703827383d3745deee1.jpg" width="690" height="388">

Added if you just want it to be separated you can just saw it off.
<img src="/uploads/db1493/original/3X/3/7/37b763f6560e18d92e51bc3d66f6a9e1749e54a2.jpg" width="690" height="388">
```

---
## \#36 Posted by: saul Posted at: 2016-12-13T22:56:07.094Z Reads: 114

```
thanks I need to print out a case and it will be ready for some real tests!

I need to learn pcb design, a custom board will make it so much smaller. but hard to argue with $3 nano clones.. $1 rf module and a couple hours of soldering. 

why not break out a few more pwm/analog pins? just to make it more flexible! I could see other uses for this! 
right now mine is controlling a mini robot.
```

---
## \#37 Posted by: Sander Posted at: 2016-12-13T23:08:10.795Z Reads: 128

```
[quote="saul, post:36, topic:14608"]
why not break out a few more pwm/analog pins?
[/quote]

Will do :slight_smile:
But I will keep making it tomorrow because its late here time for bed.
Good night![quote="saul, post:36, topic:14608"]
I need to learn pcb design, a custom board will make it so much smaller. but hard to argue with $3 nano clones.. $1 rf module and a couple hours of soldering.
[/quote]

 Mhmm from oshpark you get this pcb with the vedders switch for 15 dollar for 3 pieces. And the Atmega around 0.9 dollar, same with the SMD nrfl24l01, and the crystal is very cheap too, but you will need 22uf for the crystal etc. But I can make it home and ship it. But that wont be before I am finished with this circuit etc. So this custom circuit will cost around 10 dollars(IF you dont want to have the switch spark because the transistors on it, is a bit expensive). Not bad for beeing a custom :stuck_out_tongue: 

What I mean with the 10 dollar price is.
IF its without the top piece(vedders switch)
ATMEGA328P-AU, can be found for 0.9 piece
NRF24L01 smd 1 dollar
Crystal <1dollar
Custom circuit for 3 = 15 / 3 = 5

5 + 3 = >9 Dollar.

There are no protection of over voltage! 
So if you are gonna use it with batteries but not with the VESC then you need a 5 VOLT battery.
Because the 3.3 Regulator only works from 4.5v -> 7v. And the ATMEGA328P-AU Chip only operate from 1.5v -> 5.5v
So I think I shall add that you can have +12v because that would be handy. But that will wait for tomorrow
```

---
## \#38 Posted by: lox897 Posted at: 2016-12-13T23:25:40.332Z Reads: 117

```
You might as well just put the VESC on there while you are at it lol.
```

---
## \#39 Posted by: Sander Posted at: 2016-12-13T23:29:06.253Z Reads: 123

```
[quote="lox897, post:38, topic:14608, full:true"]
You might as well just put the VESC on there while you are at it lol.
[/quote]

Haha! I was planning on making a motherboard for my eboard. Also all in one pcb. Li-ion Bms 12S charging, 2 VESC, Vedders Switch, and the hardware I use(ATMEGA, NRF24L01, BT and the Neopixel Lights).

But recreating the VESC takes a lot of time and I saw the VESCX has alot less components then the VESC.

Well maybe after christmas I will create a motherboard for my eboard :stuck_out_tongue:
```

---
## \#40 Posted by: saul Posted at: 2016-12-13T23:38:15.832Z Reads: 119

```
This save time cutting wires and soldering, plus its much more compact so its worth it!!
no rush! my prototype boards will work fine for testing the software.
```

---
## \#41 Posted by: Sander Posted at: 2016-12-14T17:34:40.287Z Reads: 120

```
[quote="saul, post:40, topic:14608, full:true"]
This save time cutting wires and soldering, plus its much more compact so its worth it!!no rush! my prototype boards will work fine for testing the software.
[/quote]
Indeed!

Update: 
<img src="/uploads/db1493/original/3X/8/0/8069821b2d79a3f259a8c26374a1aec510815def.jpg" width="690" height="388">
```

---
## \#42 Posted by: Sander Posted at: 2016-12-17T12:52:27.066Z Reads: 112

```
Found a way to get rid of those holes with using the slot and force solder mask over it!
And made the ports at the bottom symmetrically.

Top:
<img src="/uploads/db1493/original/3X/c/6/c6c9eb5422d70db5425fd2943138ab9b0954e744.jpg" width="690" height="388">

Bottom:
<img src="/uploads/db1493/original/3X/0/3/038c1cfb3b90fe713936ede8e787d2a988a7537d.jpg" width="690" height="388">

Inside:
<img src="/uploads/db1493/original/3X/e/3/e3bd328d31f6996b0ae7f0ebc1696c7b7c89f9f2.png" width="690" height="388">

Question:
Is it smart to have the ground plane to the edges?
Or should I have a little space between the edge with the ground plane?
```

---
## \#43 Posted by: saul Posted at: 2016-12-17T21:46:16.828Z Reads: 100

```
[quote="Sander, post:42, topic:14608"]
Question:Is it smart to have the ground plane to the edges?Or should I have a little space between the edge with the ground plane?
[/quote]

This is looking really awesome! but i have no experience with pcb design for now. maybe @chaka can help out?
```

---
## \#44 Posted by: Sander Posted at: 2016-12-18T13:42:39.203Z Reads: 92

```
<img src="/uploads/db1493/original/3X/0/8/08dc32adf298a2868a7605f7d3b1a43fff8693fc.jpg" width="690" height="152">

With the SparkSwitch Circuit, Bluetooth, MOSFET it will cost 28.3 dollar for one to make.
Without bluetooth and the vedder's spark switch it will cost 17.59 dollar to make one.
```

---
## \#45 Posted by: rwxr Posted at: 2016-12-18T13:51:43.436Z Reads: 92

```
Are you going to produce complete boards, kits or just open source it?
I have some hookups with companies that can make either just PCB's or complete boards in sweden. Let me know if you want me to ask them for estimates.
```

---
## \#46 Posted by: chaka Posted at: 2016-12-18T17:55:13.309Z Reads: 90

```
It is good to end the ground plane before the edge of the board. There are several reason as to why but it is a good habit to have when finalizing your gerber files to have a small border free of copper.
```

---
## \#47 Posted by: Sander Posted at: 2016-12-18T19:27:52.632Z Reads: 98

```
[quote="rwxr, post:45, topic:14608"]
Are you going to produce complete boards, kits or just open source it?I have some hookups with companie
[/quote]

I am not really gonna produce like for people to buy but if they as I can make for them.
But I am defintley gonna make the PCB for me! And yes ask the companies I wonder how expensive they are :) Because I live in the neigbour country(norway)
```

---
## \#48 Posted by: Sander Posted at: 2016-12-18T19:28:00.568Z Reads: 95

```
I thought so! Thanks ;)
```

---
## \#49 Posted by: Sander Posted at: 2016-12-22T01:56:29.664Z Reads: 101

```
<img src="/uploads/db1493/original/3X/4/4/44d2ab80742f8bb344cbae399979d8730b88c812.jpg" width="690" height="388">

Its much much compact and smaller!
The boad under the AntiSpark(Vedder's Switch) is 28.14x16.33mm
And if you would only order that piece it would only cost 3.55 dollar for 3!
But with the vedder's switch it cost 14.5 dollar for 3.

And now the circuit can have 1.8->16 volt in the power. It will be converted to 3.3V for the 2,4ghz transciever, and I removed bluetooth.
```

---
## \#50 Posted by: saul Posted at: 2016-12-22T10:11:08.238Z Reads: 98

```
That looks awesome. :nerd:

I've been working with my perfboard version on this, need to clean up and post the code.
already have turnsignals, brakelights and random sequenses from a separate module. 
Just need to make sure there are enough failsafes and add some throttle ramping. 


is there an antenna for the nrf? the integrated one on these cheap module work great at short range < 10m.
```

---
## \#51 Posted by: Sander Posted at: 2016-12-22T18:36:15.490Z Reads: 97

```
[quote="saul, post:50, topic:14608"]
is there an antenna for the nrf?
[/quote]

<img src="/uploads/db1493/original/3X/9/c/9c7de753375d69e42c6b6352d90560b147535e02.jpg" width="666" height="500">

Its the one on right.
The turn lights sounds awesome I was considering on making that. Because on my controller I will add many more functions, like it will be easy access to hit a button that makes it blink to left or right and I will have brake lights etc.

I will start developing it when I have made my Resin Printer.

NRF24L01:
It has an inbuilt antenna but the range depends on library etc.
And I have had over 20m no problem. And I will look for the best library for maximum range and I will add protocolls etc so you will not get any interference problems.
```

---
## \#52 Posted by: saul Posted at: 2016-12-22T19:42:53.226Z Reads: 92

```
I've been using the version on the left since its more breadboard friendly. Its gone much further on my rc car but it really only matters for short distance on esk8...

Did you get a form2? 
I already have a bunch of 3d models for remotes, resin could do even more details i'm sure.

if you're going no bt, i would break out rx, and tx pins so you can relay vesc data to a remote screen.
its just 2 pins and a bit more code so why not right? :nerd:
```

---
## \#53 Posted by: Sander Posted at: 2016-12-22T20:05:01.399Z Reads: 99

```
[quote="saul, post:52, topic:14608"]
if you're going no bt, i would break out rx, and tx pins so you can relay vesc data to a remote screen.its just 2 pins and a bit more code so why not right?
[/quote]

The TX and RX are already breaked out :)<img src="/uploads/db1493/original/3X/0/6/06d1c57d1fe4ee3eb57ee4f5453af0b20e477290.png" width="436" height="500">
But the TX and RX is inverted also TX are arduino RX and RX is arduino TX because of the FTDI Usb has it like that.

[quote="saul, post:52, topic:14608"]
Did you get a form2?
[/quote]

No its too expensive for me :sweat_smile:
I am making my own, with my own hardware.
I think I will make it bot to top resin printer.
It's really easy to make all you need is a UV Projector, and a Z-Axis stepper motor.
Some coding with the gcode files about when it shall move up. And I will make it like it fills the resin after it has used some so the resin usage will be minimal and it will swipe over after it has cured because of better results etc.

The cost of steppers etc and all electronics will be around 30 dollars.
For the projector around 299 dollar for a really good and high quality projector.
And resin cost around 30?

So The Resin printer will cost around 400 dollars then 2000 dollar.

I have seen many homemade resin printers, the quality is the almost as same as the Formlabs,
But it depends on how far your projector is, focused etc...

This is an example, you see how simple it is?
https://www.youtube.com/watch?v=DhXa6Q1JJH0
https://www.youtube.com/watch?v=KOqZiRZM5pk
```

---
## \#54 Posted by: Sander Posted at: 2016-12-22T21:05:37.099Z Reads: 90

```
And Im gonna make a pick and place machine with automatic reflowing, and automatic solder on the pads.<img src="/uploads/db1493/original/3X/c/f/cf37a2f6b0d7435a11df1fb7d6bb5ae13b48f0b6.jpg" width="690" height="430">
This is the thing I will build on.
```

---
## \#55 Posted by: saul Posted at: 2016-12-22T22:57:11.455Z Reads: 88

```
Mmm that's pretty interesting. I have a reprap i3. Works fine but projectors have gotten cheaper since then.

I've been wanting to do a pick and place for a while but I wasn't sure where to start.

I was thinking a infra toaster mod for reflow and pick and place separately.
```

---
## \#56 Posted by: Sander Posted at: 2016-12-22T23:23:41.528Z Reads: 88

```
[quote="saul, post:55, topic:14608"]
I was thinking a infra toaster mod for reflow and pick and place separately.
[/quote]

Yes, the toaster is better and if you "hack" it so it goes by the rules of the solder pasta with right temperatur.

But this is just an idea for the future in 1-2 years, when I get better with coding and making softwares.
I started with electronics/coding for 8 months ago as my hobby(still my hobby, I'm still in middleschool lol) and I have come pretty far on so little time.
So I wonder how much I can do when I have created CNC Machine, Resin Printer etc.
```

---
## \#57 Posted by: Sander Posted at: 2016-12-23T21:00:50.560Z Reads: 85

```
Well here is the same with my design of the spark switch:
<img src="/uploads/db1493/original/3X/7/f/7f48932af18cc880b586878cbcb7a20e273c5e36.png" width="519" height="500">
```

---
## \#58 Posted by: Sander Posted at: 2016-12-23T21:37:34.151Z Reads: 89

```
Before it costed 14.5 dollar for 3 pcb.
Now it cost 9.25 dollar for 3!

If its smaller its cheaper!
So each board cost around 3 dollars.

And you can see I have breaked out the TX and RX on the bottom.

<img src="/uploads/db1493/original/3X/e/7/e7391ca85d475fcdf4e511b87c8bd47cf66d69b5.png" width="500" height="483">
- BORDER - BORDER - BORDER - BORDER - BORDER - BORDER - BORDER -
<img src="/uploads/db1493/original/3X/d/a/dac161edd4cb90bce8039131b76a9859994b43f1.png" width="500" height="483">
```

---
## \#59 Posted by: saul Posted at: 2016-12-28T07:31:06.014Z Reads: 82

```
really cool. you can see the progression you've made from the first post to this.

a single fet makes it really compact, but it might get too hot. 
not sure how to solder a directFet but seem like they are they way to go now since you can easily add a heatsink and keep the pcb compact. short traces.
```

---
## \#60 Posted by: Sander Posted at: 2016-12-28T13:51:35.493Z Reads: 83

```
The mosfet is on both side, but yeah, it might be hot. But you never know until you try xD ;)
```

---
## \#61 Posted by: Sander Posted at: 2017-01-27T19:41:57.816Z Reads: 81

```
UPDATE:

**Top of the Circuit**
<img src="/uploads/db1493/original/3X/1/6/16ff01e3293dd43a4edd32a3fa553e3d8f053a90.jpg" width="375" height="500">

**Bottom of the Circuit**
<img src="/uploads/db1493/original/3X/e/5/e5120c393e52c3ef62afd606528c7b05e19cb8a9.jpg" width="375" height="500">

**Information & Testing of the Circuit:**
I've got this for 2-3 weeks ago.
I mounted all the components with hot air.

After some testing I got it finally running.
I tested with a code that when it recieved a 1, the lights would go on, 0 lights off.
The sender had another version of the Nrf24l01, I was worried it wouldn't be compatible but it was ;)

I was testing the power input with 11.1V and it did the job, lower the voltage to 3.3V!
I have shorted the circuit a few times, it smoked. But I didnt destroy any of the circuit only a lane in the copper where the ground is input, that's why I have a black wire going to both of the grounds.

**Range Test:**
I did a range test with having one in my room and the other in the living room, around 20-25 meter distance. It worked perfect! And responsed way faster then my expectations!

**Uploading the Code:**
To upload the code you just connect to the pins with a ftdi usb to serial port.
You chose the card with the processor in the Arduino IDE(Arduino Pro Mini)
Then the COM port of the ftdi.
Press upload, then done!

**Vedder Switch At Top:**
The Switch works perfect! 
Turns of the power and on like it should do!

I'm gonna make a new Vedder Switch with a momentary push button!
What I mean is when you press a momentary button it turns on an IC,
When the IC is on it keeps the gate of the MOSFET on until you press the button again!

You can change the settings with how long you shall hold the button for it to turn on/off,
with using a jumper between two pins or a button with 4 position?

I will start sketching/testing it soon.

**Some Regrets:**
The green led on the left of the red led that indicates the power should not have been set to pin 13.
Because the Nrf24l01 is using that pin for sending/recieving so I have no controll of it. I rather should have chose D8 pin. But it actually shows when its reading, the green led is flickering so fast that it looks its on with a very low brightness ;)

**My Carbon Board(Almost Finished)**
<img src="/uploads/db1493/original/3X/8/6/86e374a28bf1ffdf27ed439d6716c61e15b2b4d7.jpg" width="375" height="500">

**Thickness 2.8 cm**
<img src="/uploads/db1493/original/3X/2/0/20ee849d241f5360805d82b26adefae15a86f354.jpg" width="375" height="500">

**With The Cover On**
<img src="/uploads/db1493/original/3X/5/1/519220139709ee757e9cd7837f06c96cb44f5d40.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/6/3/632c7c122bcaf4f5cbc109aad0d6b08625ae4fee.jpg" width="666" height="500">

<img src="/uploads/db1493/original/3X/d/c/dcee826249fef92cbbdced3584df893f0b1d7c6d.jpg" width="375" height="500">

<img src="/uploads/db1493/original/3X/1/b/1b69feb1a9fdc5ec2c4df83de9bb69b8505cbd4d.jpg" width="666" height="500">

**Carbon Board Info:**
The board is cut out in wood, then later wrapt in carbon.
The carbon process took about 1 week.

All that is left to do on the board is to drill a few holes for the wires to the motor and for the on switch.
```

---
## \#62 Posted by: Sander Posted at: 2017-01-29T15:25:01.963Z Reads: 68

```
**Video:**

https://www.youtube.com/watch?v=SQ7KS-jgceU

I have made that it has a slow acceleration but fast down accelration, like when you shall brake
```

---
