# Bluetooth battery monitor

### Replies: 69 Views: 4874

## \#1 Posted by: chinzw Posted at: 2016-10-25T15:35:53.796Z Reads: 325

```
Hey guys, so I wanted to keep my build as clean and stealth as possible, so im building an around based BT monitor.
Prototype already working, now I just need a nice guide for mobile.

<img src="/uploads/db1493/original/3X/d/c/dcef509a5668fef3bfd0959a38b7ce6a7cf5bb62.jpg" width="666" height="500">
<img src="/uploads/db1493/original/3X/5/b/5b6aab59e82501d1dfee8457f238cd746b3261ba.png" width="281" height="500">

I will be posting schematics and everything else if anyone is interested.
```

---
## \#2 Posted by: Hummie Posted at: 2016-10-25T15:57:03.705Z Reads: 285

```
Cool what is it exactly?  Ideally I'd like my 12 cells shown on my phone  .
```

---
## \#3 Posted by: Aborn Posted at: 2016-10-25T15:58:06.915Z Reads: 283

```
Teensy! <3

A wild guess is it's just a bunch of voltage dividers and then Analog input for each cell from the balance connector on the pack. And a bluetooth module,

I can only see one voltage divider tho, not quite sure how that works, since i can see the battery level of the indivudal cells on your screenshot
```

---
## \#4 Posted by: Hummie Posted at: 2016-10-25T16:00:24.114Z Reads: 272

```
Sounds great does it run off a bec?  Iphone?
```

---
## \#5 Posted by: Aborn Posted at: 2016-10-25T16:02:59.472Z Reads: 261

```
The teensy can run of 5V which a bec supllies, or 3.3 V.

So it runs off the ubec, and connects with the phone
```

---
## \#6 Posted by: evoheyax Posted at: 2016-10-25T16:03:33.072Z Reads: 260

```
Injteresting idea. I wonder if you could bundle the data up with the vesc data. My app does battery monitoring of the overall battery, but not individual cells.
```

---
## \#7 Posted by: Aborn Posted at: 2016-10-25T16:04:36.930Z Reads: 256

```
Monitoring the individual cells isnt really neccesary anyways. :slight_smile: ireally like the idea though.

How are you going to comprimise it?
```

---
## \#8 Posted by: Hummie Posted at: 2016-10-25T16:04:46.260Z Reads: 253

```
If so that would be ideal.  maybe u two could make it hapoen!
Maybe a simple alarm when a cell hits a low voltage
```

---
## \#9 Posted by: Aborn Posted at: 2016-10-25T16:06:42.182Z Reads: 240

```
It shouldnt be too hard, the circuit is very simple, Bluetooth modules are cheap. The microprocessor could be replaced by one of the [tiny arduino chips](http://www.ebay.com/itm/5PCS-ATTINY85-20PU-IC-MCU-8BIT-8KB-FLASH-8DIP-New-/281682083949) something like that.
```

---
## \#10 Posted by: evoheyax Posted at: 2016-10-25T16:06:43.880Z Reads: 232

```
I get all my data straight from the vesc through the uart port. This includes battery overall voltage.
```

---
## \#11 Posted by: Aborn Posted at: 2016-10-25T16:07:21.955Z Reads: 228

```
Ah, and how do you transmit it to your phone?
```

---
## \#12 Posted by: evoheyax Posted at: 2016-10-25T16:09:40.999Z Reads: 228

```
I use the adafruit BT 4 LE UART friend chip. Pretty simple to use actually. Thanks to the rollingGheko, the bluetooth code was already written, so for me, it's just programming what to do with the data once the iphone has it.
```

---
## \#13 Posted by: smudgeUK Posted at: 2016-10-25T16:11:21.097Z Reads: 229

```
<img src="/uploads/db1493/original/3X/6/7/6711736752afee1eb274f1c3e5fa7f61fb3a8333.jpg" width="375" height="500">

Snap ! :slight_smile:
```

---
## \#14 Posted by: Aborn Posted at: 2016-10-25T16:12:24.003Z Reads: 220

```
Alright what do we got here. Arduino, Bluetooth, a display, some leds and a potentiometer.. Hmm what does it do? xD

Again battery monitor with both display, bluetooth and leds to display the voltage? O.o
```

---
## \#15 Posted by: smudgeUK Posted at: 2016-10-25T16:14:08.617Z Reads: 212

```
Haha eagle eyes :slight_smile:
its still in its 'proving the idea phase' ...
if @chinzw doesnt mind me jumping in with him on this thread i dont mind explaining a little more. Its along the same lines
```

---
## \#16 Posted by: chinzw Posted at: 2016-10-25T16:54:39.688Z Reads: 208

```
@smudgeUK not mind at all!

Im using voltage dividers on the analog inputs, which is pretty simple given the nature of 4.2,8.4... so the dividers are like 10k/20k, 10k/30k... etc. With a nano im limited to 8 analog pins, this can be increased by using an CD74HC4067 analog muxer.

EDIT: i will add some LED outputs to display the state of charge of the whole battery too.
```

---
## \#17 Posted by: smudgeUK Posted at: 2016-10-25T17:12:22.460Z Reads: 217

```
Ok thanks ! maybe we can bounce ideas and get some inspiration/help from each others projects :-)
Firstly, im learning arduino as i go, this is really my first proper project with it besides messing with some basic code and circuits a few months ago. Im getting there i think. Ive got decent electrical knowledge but my electronics/coding certainly lacks.

Mine is in the early (testing) stages. Im looking at monitoring individual cell voltages and system component temperatures ... via bluetooth (on request), on the lcd screen and via leds. I have 3 leds marked 'batt , esc , motors' and an ok led and a fault led.
Through the loop the cell voltages will be displayed on the screen, then the temperatures of the components. If my set parameters are reached for voltages or temps, at the end of the loop the fault led flashes along with the corresponding led for the component (+batt led for low voltage or high temp, or maybe the fault led along with motor led if the motor reaches a certain temp). There is also an error message on the display saying where the problem is. 
My future idea was to have the 5110 as a HUD running wirelessly with a nano + bluetooth (multiple bluetooth modules together - im not sure if its possible). Obviously this would be much safer/easier than looking down at the board when riding or even having to stop.

A few points up to now:

-My picture only shows one pot being used to prove the reading works via bluetooth to my phone. It works great, but now i need to work on cells 2+ due to, as you say, needing voltage dividers.
The app im using allows the buttons on screen to be named and also the command they send to be changed. This means i can add up the individual voltages in the arduino and output it, when requested, by clicking a button in the app. This would then tell me the total pack voltage on my phone.

-I have a ds18b20 probe connected to a seperate arduino that im working on as im struggling with correct resolution for the probe reading. Possibly a library mis match im not sure ...
 Other things im sure but ive just got up (working nights) and havent had 5 cups of coffee yet :-)
```

---
## \#18 Posted by: Aborn Posted at: 2016-10-25T17:13:56.349Z Reads: 198

```
You dont even need voltage dividers if you're going to measure all of the cells, you just need a lot of Analogin Input pins
```

---
## \#19 Posted by: chinzw Posted at: 2016-10-25T17:19:11.665Z Reads: 212

```
well, you do, unless you want to fry your I/O ports, gnd to cell 1 is 4.2, but gnd to cell 2 is 8.4, boom bye bye port.

@smudgeUK check the marlin repo, we use temp sensors for the hotends and heated bed. Not all sensors have the same resistance or curve, so you need to work that in.
```

---
## \#20 Posted by: Aborn Posted at: 2016-10-25T17:20:23.131Z Reads: 210

```
If you measure between the cells like this

<img src="/uploads/db1493/original/3X/b/0/b0f4edf3022ccd991f83ac1814c0bd96d04e3222.png" width="690" height="461">

You can get the voltage of the cells indivudally

**+1 for paint skills**
```

---
## \#21 Posted by: chinzw Posted at: 2016-10-25T17:36:40.782Z Reads: 188

```
You cant do that with an arduino, the I/O pins measure from common ground.
```

---
## \#22 Posted by: Aborn Posted at: 2016-10-25T17:37:16.158Z Reads: 178

```
Ohhhhh yes you are right :frowning:
```

---
## \#23 Posted by: chinzw Posted at: 2016-10-25T18:04:27.894Z Reads: 178

```
It runs of a buck dc-dc, can be a 5v ubec (its pretty much the same) at the moment is 8s max, but with a analog mux it can be increased to 12s+. At the moment im using a bluetooth serial app, which you can find for android/iphone, and it will show you the cell voltages in numerical format. Im planing on writing an app that has a nice ui to display all the data.
```

---
## \#24 Posted by: chinzw Posted at: 2016-10-25T18:14:42.729Z Reads: 177

```
Another thing im considering for reading more cells would be this:
http://ww1.microchip.com/downloads/en/DeviceDoc/21298e.pdf

which free's up the digital i/o pins for other uses as it connects to SPI
```

---
## \#25 Posted by: smudgeUK Posted at: 2016-10-25T19:15:02.953Z Reads: 181

```
Yes this was my concern ! I knew i would run into problems after the first cell ... but i wanted to see if i could actually do one cell first :-) haha.
Im only running 8s anyway so this would suffice !
@chinzw Ive got the actual cell voltage displayed on my bluetooth app too. The buttons in the app are configurable both in their labelling and their command sent to arduino so for an already made package, its pretty good. Ill get a screenshot in a bit and show you what ive currently got, and also get the name of the app. Which app are you using?
```

---
## \#26 Posted by: saul Posted at: 2016-10-25T19:27:17.294Z Reads: 178

```
cool, you can use an arduino nano and analog mux 16ch. so you can have 12 voltage dividers no problems ;)

a bit more code but still cheaper than a teensy.
```

---
## \#27 Posted by: smudgeUK Posted at: 2016-10-25T19:35:56.286Z Reads: 184

```
<img src="/uploads/db1493/original/3X/5/b/5b7c40676d01c4a6385e1e4d89be7eb9340ce87f.png" width="281" height="500">
```

---
## \#28 Posted by: chinzw Posted at: 2016-10-25T21:10:29.309Z Reads: 175

```
Im using that exact same app. But im gonna do a cross platform app so that i can also do the monitoring on my win, mac or linux boxes.
This morning i connected the charger reversed (its a really bad 2 pin waterproof connector which is going in the trash) so i had to monitor the cells to make sure the BMS wasn't fried, it would have been great to have this all done lol!
```

---
## \#29 Posted by: smudgeUK Posted at: 2016-10-25T21:31:21.741Z Reads: 168

```
I guess you want that to monitor charging levels etc while at home?
BT and a visual on the board would be fine for me. The rest of the cells will be something i need to work on in the future. I have a few other bits to add to the circuit as long as i have pins left :-/
Going to be diving into some more complicated things on arduino soon once ive got to grips with this part. Myself and @EssEnn have been discussing various possibilities via pm. Maybe its time for a dedicated arduino thread ...
```

---
## \#30 Posted by: chinzw Posted at: 2016-10-25T21:33:14.661Z Reads: 169

```
I've also been thinking how i can hack my BMS to read if its bleading, charging, etc. Need to do some more research on BMS which i lack some knowledge.
```

---
## \#31 Posted by: smudgeUK Posted at: 2016-10-25T21:38:20.466Z Reads: 156

```
Once you have your inputs all working then im sure most things are possible in the code ... you can play about with rates of increase/decrease as you please.
Im thinking of running my arduino off x2 18650s but not sure if this is the best idea or not
```

---
## \#32 Posted by: chinzw Posted at: 2016-10-25T21:41:26.037Z Reads: 153

```
Just run it from the main battery, no need to add more batteries you need to take out and charge. Plus 2x18650 = 8.4v, too high for arduino so you will need a buck converter anyways. Ill be wiring 2 circuits to power the arduino, one powers when the VESC is on and the other one powers with its own switch, that way i can monitor cells when charging and when riding.
```

---
## \#33 Posted by: chinzw Posted at: 2016-10-27T07:17:08.380Z Reads: 166

```
Got my delivery from digikey! 1% resistors ftw :slight_smile:
All the code is done for the battery monitoring, supports as many cells and LEDs as you can plug in and is 100% scalable. Min and Max voltages can be set also to set the range of the LEDs. 

Here im using 3S since i dont really have a bigger protoboard lol, ill have to buy another small one and stack them.
<img src="/uploads/db1493/original/3X/c/c/cc7824b32976fa80e7c68ef406b79fe9f87d8994.png" width="281" height="500">

<img src="/uploads/db1493/original/3X/5/4/54080c05fee408cd30a040e84cc2b183d8e718d6.jpg" width="666" height="500">
```

---
## \#34 Posted by: smudgeUK Posted at: 2016-10-27T09:39:41.018Z Reads: 152

```
Im sure i saw my nano can handle 7-12v input ...
Good job on the readings, im still waiting on my divider circuits to be delivered so i can sort cells 2-4 out, damn postal service :-(
```

---
## \#35 Posted by: chinzw Posted at: 2016-10-27T15:52:39.279Z Reads: 142

```
I was powering ditectly to the 5v raíl for accuracy test. Now im using 8v on vin
```

---
## \#36 Posted by: chinzw Posted at: 2016-10-30T04:48:29.534Z Reads: 149

```
First prototype! Need to add another JST for the VESC.
<img src="/uploads/db1493/original/3X/1/b/1b7b26c17f654a437aec41e87794d9d3db6e48b6.jpg" width="374" height="500">

I will soon do the schematic/PCB when I have some spare time.
```

---
## \#37 Posted by: chinzw Posted at: 2016-10-30T10:10:47.237Z Reads: 153

```
VESC UART port added, just need to go get some micro jst connectors tomorrow morning to hook everything up :slight_smile:

<img src="/uploads/db1493/original/3X/c/5/c57c0eff43af2484faf3ca8ed6e7f8bea68ca7d7.jpg" width="666" height="500">
```

---
## \#38 Posted by: chinzw Posted at: 2016-10-30T19:34:24.923Z Reads: 154

```
All hooked up! Couldnt get the micro JST, its Sunday doh!
<img src="/uploads/db1493/original/3X/a/6/a628e309296793354b2d33f475d73b5c993caed5.jpg" width="666" height="500">
```

---
## \#39 Posted by: smudgeUK Posted at: 2016-10-30T22:15:09.898Z Reads: 154

```
Very neat work ! Nice :-)
```

---
## \#40 Posted by: chinzw Posted at: 2016-10-31T08:45:09.172Z Reads: 151

```
All done! (Well, still no micro jst, but all wired up, case done, tested and calibrated the arduino readings.

<img src="/uploads/db1493/original/3X/9/2/928f22b0dc1716a6265c9ded536b616c4755ec58.jpg" width="375" height="500">
```

---
## \#41 Posted by: Aborn Posted at: 2016-10-31T19:26:23.911Z Reads: 135

```
Did you make it compensate for voltage drops?, if not, you should!
```

---
## \#42 Posted by: 2-alex-2 Posted at: 2016-10-31T19:47:13.720Z Reads: 132

```
Very nice but for me day to day riding I wouldn't use its at all but nice to have for day once a month to check on the levels and to make sure the bms is doing its job. Would it take Mich to make this to sell as I would buy one if was a little more compact.
```

---
## \#43 Posted by: chinzw Posted at: 2016-11-01T04:42:31.168Z Reads: 126

```
I am compensating for voltage drop across the whole circuit. But i don't have a precise enough measuring tool for such small voltage drops so i haven't been able to corroborate the numbers to precisions higher than 0.01v
```

---
## \#44 Posted by: chinzw Posted at: 2016-11-01T04:57:31.035Z Reads: 135

```
[quote="2-alex-2, post:42, topic:11867, full:true"]
Very nice but for me day to day riding I wouldn't use its at all but nice to have for day once a month to check on the levels and to make sure the bms is doing its job. Would it take Mich to make this to sell as I would buy one if was a little more compact.
[/quote]

It takes me 2 seconds to check the voltages form my phone to make sure everything is working as intended, it gives me peace of mind (specially since im using lipos). Also, i can keep logs of cell status, etc. And it the software will also give status info on the VESC which is usefull.

I am in the process of making schematics and pcb for this project. Im trying to lay everything out as compact as possible and ideally single layer pcb so anyone can etch/mill their own. Im still trying to find a 12 channel through hole ADC, but its proving hard to find, might use a smd 12 channel but that might complicate some people who are not too good at soldering.
If i got the SMD route, i can make everyting REALY small.
```

---
## \#45 Posted by: jmasta Posted at: 2016-11-01T06:13:27.348Z Reads: 127

```
Very cool @chinzw!
```

---
## \#46 Posted by: 2-alex-2 Posted at: 2016-11-01T09:12:24.394Z Reads: 127

```
Yea I think smaller the better for something like this but have a larger diy version maybe for people with out the capabilities to solder smd.
```

---
## \#47 Posted by: chinzw Posted at: 2016-11-01T22:13:06.885Z Reads: 118

```
With the right component selection smd would be as easy as soldering through holes. The only "difficult" thing is the 12 channel adc.
```

---
## \#48 Posted by: Aborn Posted at: 2016-11-02T00:07:28.908Z Reads: 124

```
Not sure if you understood what i ment.

What i mean is, when you drive the board, and start pulling power from the battery, you get a very large voltage drop on the battery, are you compensating for this?
```

---
## \#49 Posted by: chinzw Posted at: 2016-11-02T00:09:47.531Z Reads: 121

```
Not really, why would you want to read anything else than the actual battery voltage? If the voltage is sagging under load, you want to know that.
```

---
## \#50 Posted by: Aborn Posted at: 2016-11-02T00:12:20.253Z Reads: 115

```
Well, if your pack is on lets say 30 V, then you accelrate and it drops to 23, when you're then up to speed it will drop less and go back to let's say 27, then when you hold still you're on 29,8 V. You wont get a precise reading (While riding at least) if you're not compensating for the voltage drop.
```

---
## \#51 Posted by: chinzw Posted at: 2016-11-02T00:14:11.896Z Reads: 104

```
Im not sure i understand what you're trying to tell me.
```

---
## \#52 Posted by: Aborn Posted at: 2016-11-02T00:17:25.535Z Reads: 108

```
All batteries drop voltage under load. The bigger the load the more the voltage drop.
```

---
## \#53 Posted by: chinzw Posted at: 2016-11-02T00:19:50.794Z Reads: 107

```
Yes, we are all clear about that. And if im going uphill full duty and my battery sags to 20V i want to see those 20V on my battery monitor. Why would i want to see any other "corrected" value?
```

---
## \#54 Posted by: Aborn Posted at: 2016-11-02T00:21:32.197Z Reads: 106

```
Because it will say your battery is on 50 % when it might be on 80 %, and i'd like to see the actual range i have left, rather than what voltage it is on at this specific load.
```

---
## \#55 Posted by: chinzw Posted at: 2016-11-02T00:24:15.322Z Reads: 107

```
Its a cell voltage monitor. Battery charge level is a whole other thing. It can be implemented, but that's not on my list any time soon.
```

---
## \#56 Posted by: Aborn Posted at: 2016-11-02T00:25:16.038Z Reads: 108

```
Alright, just wanted to tell you, it would be a neat feature.
```

---
## \#57 Posted by: chinzw Posted at: 2016-11-02T06:03:56.728Z Reads: 116

```
The math to calculate voltage sag is incredibly complex, and very dependant on soooo many factors it would be quite hard for the average user to set up properly. You need to take EVERYTHING into account, batteries (type, age, cycles), every resistor,  transistor, cap, mosfet, pcb trace, wire, solder job, etc, etc, etc... its not something that can just be done and work for everyone.
```

---
## \#58 Posted by: chinzw Posted at: 2016-11-03T06:27:32.936Z Reads: 111

```
Made a quick python app for monitoring the cells from a PC, will add some plotting at some point.

<img src="/uploads/db1493/original/3X/7/6/769946174aae9e184d8cd8a7b18e1af0b4061f76.jpg" width="213" height="368">
```

---
## \#59 Posted by: Aborn Posted at: 2016-11-03T18:03:50.571Z Reads: 107

```
I really like your project, might very well build it into my board, when i get to building it.

Do you need any help with the actual app?, also, will you be making it for Android or IOS?, because IOS is supposed to be expensive, for what i've heard.
```

---
## \#60 Posted by: chinzw Posted at: 2016-11-03T18:06:54.703Z Reads: 109

```
I'm redesigning the electronics at the moment, using differential op amps which should give a much more accurate reading.
Im still looking at solutions for cross platform deployment. The windows app is done in python since its quick and easy for such a simple thing.
Once i get the mobile app done, i will release the source code so that anyone can build their own.
```

---
## \#61 Posted by: themegak Posted at: 2016-11-03T19:11:15.204Z Reads: 104

```
This is something that i always wanted to be able to track from my phone.  Thanks for the doing the work and for making it available for everyone when it is ready.  Kudos !
```

---
## \#62 Posted by: chinzw Posted at: 2016-11-04T16:37:57.463Z Reads: 106

```
Aaaaaand... i blew my nano :frowning:
Trying to connect the VESC to the arduino, started getting parasite voltages and boom, goodbye nano.
Good thing is op-amps arrived and new nanos come on monday so i can start designing V2 which will isolate the balance lead inputs and prevent this from happening again.
```

---
## \#63 Posted by: chinzw Posted at: 2016-11-11T08:00:36.997Z Reads: 110

```
All back to normal, and the new implementation with differential amplifiers works much much better. Still not perfect, but very good.
Main problem with differential amplifiers is the common mode range, in the case of the LM324AN iis Vcc - 2, so when you get to the last cell of the battery, you need to use a voltage divider to get it into that range, and this adds an extra layer of error possibility.
I believe opto isolators are the way to go. They have all the positive things of op-amps and none of the drawbacks (at least in this implementation)

It doesn't look pretty, but i cant be bothered to route a pcb until i have my final design.

<img src="/uploads/db1493/original/3X/f/c/fc26ee469129330b251975da590ed6002aec2101.jpg" width="666" height="500"><img src="/uploads/db1493/original/3X/a/2/a290279ff688d259e16ec6cdb77139d4de3e3841.jpg" width="666" height="500">
```

---
## \#64 Posted by: Okami Posted at: 2017-10-18T21:30:16.318Z Reads: 62

```
This was a nice project.. to be honest, it looks like there are not that many cell meters on the market :)
```

---
## \#65 Posted by: chinzw Posted at: 2017-10-18T21:50:35.839Z Reads: 60

```
I never made a final version of this, just used the last prototype for a while but now im using pretty good bms so having this is not necesary anymore.
```

---
## \#66 Posted by: Okami Posted at: 2017-10-18T21:54:26.045Z Reads: 63

```
which one are u using? 

Im planning on implementing bms for charge only, so I still need something for low charge monitoring for each cell.. been looking and so far the best option seems to be IDST smart battery checker but im not sure yet if im ready (my friend actually) to invest 20usd to buy it.. even if it is really good.

Then again there are these loud buzzer alarms but they dont seem reliable for me and once they start beeping they are super noisy and annoying..
```

---
## \#67 Posted by: chinzw Posted at: 2017-10-18T22:07:09.239Z Reads: 61

```
Im using raphaelchang's bms and will soon start using JTAG's bms.
```

---
## \#68 Posted by: Okami Posted at: 2017-10-18T22:25:05.582Z Reads: 66

```
Good choice. Then I totally understand why u said good bms :)
```

---
## \#69 Posted by: SPAC Posted at: 2018-05-20T00:05:47.333Z Reads: 47

```
Hi, Aborn

Have a landwheel board and modifying it, 
It is not a terrible idea, To improve the skateboard with a power generator battery pack, for charging 10s 42.2v battery on the go. I was wondering if you knew how to connect bluetooth device to my phone or smart watch because while charging skateboard battery which is in my backpack it would be good to see the charging without having to stop to pull the battery out of the bag. You have a great project but could you simplify it, to monitor battery charge with bluetooth.

Good day, Great work.
```

---
