# How to make Bluetooth module? and make it work?

### Replies: 51 Views: 3142

## \#1 Posted by: stormboard1 Posted at: 2018-03-13T21:54:39.504Z Reads: 318

```
![image|375x500](upload://pD6NuN5vFAvpBDy34CcitV1cSh.jpg)Got the Bluetooth module and wire adapter but couldn’t find a thread on how to put one together.. so how do I put one together 😂
```

---
## \#2 Posted by: Deckoz Posted at: 2018-03-13T21:57:38.445Z Reads: 307

```
look at the pins on the backside of the bluetooth they should be labled on the silk screen...

connect the tx and rx 5v and gnd. to the same pins on your vesc/focbox uart port... which are either labeled on the case or on the silk screen
```

---
## \#3 Posted by: stormboard1 Posted at: 2018-03-13T22:00:32.348Z Reads: 307

```
I see the txd , rxd, god, but no 5v on the module in the pic
```

---
## \#4 Posted by: Aleks Posted at: 2018-03-13T22:00:52.826Z Reads: 299

```
while on this topic, if running dual focbox's, is a bluetooth module needed for each?
```

---
## \#5 Posted by: GrecoMan Posted at: 2018-03-13T22:01:18.413Z Reads: 294

```
use vcc instead of 5v
```

---
## \#6 Posted by: Deckoz Posted at: 2018-03-13T22:01:30.489Z Reads: 296

```
[quote="stormboard1, post:3, topic:49020, full:true"]
I see the txd , rxd, god, but no 5v on the module in the pic
[/quote]

vcc ;)

[quote="Aleks, post:4, topic:49020, full:true"]
while on this topic, if running dual focbox’s, is a bluetooth module needed for each?
[/quote]

One module, both connect via canbus
```

---
## \#7 Posted by: stormboard1 Posted at: 2018-03-13T22:05:38.769Z Reads: 289

```
Dju trim the prongs on the bt module?
Also I’m soldering to which side?the prongs or the pins?
![image|375x500](upload://3I1ZNM8tqWLzQhBI76OocTO945x.jpg)
![image|375x500](upload://xhTAMDgzsM4dZxX1rle9TvJNpAZ.jpg)
```

---
## \#8 Posted by: Deckoz Posted at: 2018-03-13T22:09:47.598Z Reads: 270

```
or desolder them...
```

---
## \#9 Posted by: thisguyhere Posted at: 2018-03-13T22:28:54.328Z Reads: 270

```
http://www.electric-skateboard.builders/t/vesc-monitor-android-app/20888

nico shows you exactly how to wire. 

I used 3pin servo cables to connect to the bt module and spliced to jst connector
```

---
## \#10 Posted by: stormboard1 Posted at: 2018-03-13T23:03:12.019Z Reads: 265

```
Ok but what do I do with “sck/adci” and “3.3v” ? And miso/adc2 not being connected doesn’t matter ya?
![image|375x500](upload://m3k0nwfs0qQqNYtdNmHAr8U3plD.jpg)
```

---
## \#11 Posted by: thisguyhere Posted at: 2018-03-13T23:07:39.296Z Reads: 245

```
correct, aside from the 4 wires specified in the instructions, the other wires are not needed
```

---
## \#12 Posted by: stormboard1 Posted at: 2018-03-13T23:09:49.715Z Reads: 247

```
What the easiest way to solder the wires ? To clip the pins or desolder them and solder to the pads? ![image|375x500](upload://vUpFZhDNOrfNFfAfpwpBEvn5XIU.jpg)
```

---
## \#13 Posted by: thisguyhere Posted at: 2018-03-13T23:15:56.538Z Reads: 243

```
I didn't solder directly to the module. 

like I said, used a 3pin servo wire to connect to module, then spliced servo wire to jst

https://fpv-flightclub.com/wp-content/uploads/3pin-servo-wire-1002.jpg
```

---
## \#14 Posted by: stormboard1 Posted at: 2018-03-14T00:24:47.661Z Reads: 236

```
Soldered up but how do I connect to it with an iPhone
Vesc vision ya?
```

---
## \#15 Posted by: Apolo Posted at: 2018-03-14T01:48:07.334Z Reads: 232

```
1. Make the module:
Foxbox side -> Bluetooth module
Tx                ->         Rx
Rx                ->         Tx
GND ->      GND
5V                ->         VCC

Notice: Tx and Rx are crossed over and switched 
I soldered directly onto the pins and heat shrinked everything. You can do it however you want since you aren't dealing with high current. 

Once your module is connected to the focbox, open up your esc tool or bldc tool and connect to the focbox
Go to app settings tab and select [PPM and UART]
Go to UART tab on the left and make sure baudrate is set to 9600bps

Download ACKMANIAC-ESC Monitor from app store and open it and turn on your board
in the app you should see a bluetooth device called HMSoft or something similar.
```

---
## \#16 Posted by: stormboard1 Posted at: 2018-03-14T01:58:36.287Z Reads: 224

```
iv the bt module soldered altough i soldered tx-tx and rx-rx first and turned it on got a soid red light..but no connection to the vesc vision app so i cheked and realised i needed to switch them to tx-rx and rx-tx now when i turn it on its flashing red instead of solid and still no connection to vesc vision..
im using iphone and ackmaniac-esc monitor doesnt show up in the app store
```

---
## \#17 Posted by: Apolo Posted at: 2018-03-14T02:10:16.449Z Reads: 213

```
Don't use vesc vision
```

---
## \#18 Posted by: stormboard1 Posted at: 2018-03-14T02:10:48.531Z Reads: 204

```
what should i use the ackmaniac one isnt on the itunes app store..man i hate iphones lol
```

---
## \#19 Posted by: Apolo Posted at: 2018-03-14T02:22:03.321Z Reads: 200

```
Have you configured your ppm and uart on the computer?
```

---
## \#20 Posted by: stormboard1 Posted at: 2018-03-14T02:22:19.300Z Reads: 196

```
ya baud 9600 and ppm and uart selected
```

---
## \#21 Posted by: Apolo Posted at: 2018-03-14T02:24:00.357Z Reads: 181

```
Does it show up on ur Bluetooth menu on ur iphone?
```

---
## \#22 Posted by: Deckoz Posted at: 2018-03-14T02:24:57.228Z Reads: 184

```
Hey dude..

Bluetooth TX goes to vesc RX
Bluetooth RX goes to VESC TX...


Uart is a full duplex bidirectional serial connection... So there must be a transmit and receive on each side..

Ie Bluetooth transmits data on TX, vesc received on RX.

vESc sends on tx Bluetooth receives data packet on RX...

Make sense?
```

---
## \#23 Posted by: stormboard1 Posted at: 2018-03-14T02:26:40.111Z Reads: 181

```
ya i know i had it wrong at first had rx to rx and tx to tx was solid red light and no connection ..swapped them to tx to rx rx to tx and now it blinks red but still no connection
```

---
## \#24 Posted by: Deckoz Posted at: 2018-03-14T02:27:47.480Z Reads: 186

```
Do you know what your module had setup?

If you have an FTDI connector and still have the header pins on, open up Arduino serial monitor and execute some AT commands to find out what the module is running on...ie if it's in master or slave mode.. what baurd rate etc


http://fab.cba.mit.edu/classes/863.15/doc/tutorials/programming/bluetooth.html
```

---
## \#25 Posted by: stormboard1 Posted at: 2018-03-14T02:29:48.542Z Reads: 180

```
i soldered straight to the pcb got rid the pins and dont have the connector anyway
```

---
## \#26 Posted by: GrecoMan Posted at: 2018-03-14T02:30:18.876Z Reads: 178

```
go into bluetooth on your phone and connect to it
```

---
## \#27 Posted by: stormboard1 Posted at: 2018-03-14T02:31:36.653Z Reads: 179

```
doesnt show up on the phones bluetooth
```

---
## \#28 Posted by: GrecoMan Posted at: 2018-03-14T02:32:17.600Z Reads: 175

```
screenshots
```

---
## \#29 Posted by: stormboard1 Posted at: 2018-03-14T02:33:50.352Z Reads: 179

```
shows up on the laptops tho i think![Screenshot (171)|690x388](upload://oTM4PXng1yYnE81JD6mfArrl5kV.png)
```

---
## \#30 Posted by: Apolo Posted at: 2018-03-14T02:52:39.611Z Reads: 175

```
Give us a picture, layout your focbox and bluetooth module connections so that we can see each wire and where they are connected to.
```

---
## \#31 Posted by: stormboard1 Posted at: 2018-03-14T03:09:15.445Z Reads: 181

```
![image|375x500](upload://dVS1K7ssn59jGn1p4Vn4bQjqf5i.jpeg)![image|375x500](upload://hLNXyallOPCrpzGvl7Yhm27zT8z.jpeg)
```

---
## \#32 Posted by: Apolo Posted at: 2018-03-14T03:10:22.982Z Reads: 173

```
Which module did you buy?
```

---
## \#33 Posted by: stormboard1 Posted at: 2018-03-14T03:19:22.972Z Reads: 173

```
got it free from @DavidBanner cause hes nice like that ..and i gotta be doing something wrong lol vesc vision should work
```

---
## \#34 Posted by: Apolo Posted at: 2018-03-14T03:31:37.412Z Reads: 173

```
This may sound dumb, but I've made this mistake before,
but did you forget to write config when you changed app settings to ppm and uart and 9600bps?
```

---
## \#35 Posted by: stormboard1 Posted at: 2018-03-14T04:04:44.359Z Reads: 173

```
nope lol wish was thst lol
```

---
## \#36 Posted by: DavidBanner Posted at: 2018-03-14T07:38:35.320Z Reads: 164

```
the modules often dont show up in the BT settings but will connect fine if you fire up the vesc monitor app.
There is a known issue with Android Oreo with low power BT devices like this
```

---
## \#37 Posted by: stormboard1 Posted at: 2018-03-14T20:10:20.161Z Reads: 155

```
ok so i downloaded the hm10 bluetooth app and it connects to bt module then and light goes solid red..going to try the eskate vesc app and see :crossed_fingers:
```

---
## \#38 Posted by: DavidBanner Posted at: 2018-03-14T20:43:36.903Z Reads: 154

```
awesome :)
```

---
## \#39 Posted by: stormboard1 Posted at: 2018-03-14T20:45:44.181Z Reads: 151

```
Downloaded the eskate vesc app but how do i connect it to the bt module?
```

---
## \#40 Posted by: DavidBanner Posted at: 2018-03-14T20:46:40.783Z Reads: 151

```
I have never used that app so I can't give you any help there I am afraid
```

---
## \#41 Posted by: GrecoMan Posted at: 2018-03-14T20:49:46.027Z Reads: 150

```
![image|281x499](upload://f2iTC1yH5V1BReKlHc5FNih61wj.png)
```

---
## \#42 Posted by: Acido Posted at: 2018-03-14T22:10:05.459Z Reads: 139

```
Cross rx and tx
Vcc us 5v
Gnd us gnd
```

---
## \#43 Posted by: Acido Posted at: 2018-03-14T22:10:27.986Z Reads: 137

```
Turn on bluetooth and location
```

---
## \#44 Posted by: stormboard1 Posted at: 2018-03-15T01:26:00.489Z Reads: 134

```
Got it nice one ya was messin round and found it lol.. the poles the same for a 6374 single motor?
```

---
## \#45 Posted by: NAF Posted at: 2018-08-08T20:08:28.548Z Reads: 96

```
@stormboard You got to help me out with my Bluetooth module. I got one right now. I've plugged it in to my vesc ..all I am getting is one light blinking ..I can't see this module with my Iphone. 

Do I need to setup something with BLDC Tool first ?
```

---
## \#46 Posted by: stormboard1 Posted at: 2018-08-08T21:50:31.902Z Reads: 93

```
@NAF ages since i set it up but the app you want is the eskate vesc app it isnt free but worth it and then if you screenshot it when the app opens ill have a better idea
@GrecoMan help this man out bro
```

---
## \#47 Posted by: GrecoMan Posted at: 2018-08-09T13:21:31.190Z Reads: 84

```
enable uart and ppm in bldc tool
```

---
## \#48 Posted by: NAF Posted at: 2018-08-09T23:07:39.834Z Reads: 80

```
@stormboard1 
Ok so I 've made some progress:

1.I've updated my VESC firmware to the most recent one.
2.I've selected PPM & UART in the menu.
3.My baudrate is set now to : 9600 because I've read somewhere here that this is the value I am supposed to have for my module.
4. I've downloaded eskate Vesc app...and it my BLUETOOTH module finally showed up - it is named as **HMSOFT** ...but at the bottom of the app it says "UNSUPPORTED VERSION" 
5. After I connect to HMSOFT - the light on my bluetooth module is constant .it's green but it's not blinking it's just constant.

Don't know what else can I do here..my VESC firmware version is: 3.39
```

---
## \#49 Posted by: stormboard1 Posted at: 2018-08-09T23:58:37.465Z Reads: 79

```
hmmm everything sounds right except the hmsoft where did you buy the bt module? my said HM10 along with most peoples.. @scepterr @GrecoMan @b264 @Clonkex anyone able help?
```

---
## \#50 Posted by: Clonkex Posted at: 2018-08-10T00:28:46.509Z Reads: 81

```
What module did you get? If you're not sure a photo might help us identify it :+1:
```

---
## \#51 Posted by: NAF Posted at: 2018-08-10T17:12:29.423Z Reads: 71

```
Ok so I did some more digging and that HMSOFT name is normal for my Bluetooth module. I got it from Aliexpress. So I've managed to connect my module to app that someone posted here a while ago : TELEMATICS - great app ..my bluetooth connected and it all seem to work.

![IMG_0617|281x500](upload://hvUG1ZI1IJ8RoLXtWBdthxssJP7.PNG)![IMG_0618|281x500](upload://gbQKyCyYmMk7Lved2OLrGZS2C6h.PNG)
```

---
