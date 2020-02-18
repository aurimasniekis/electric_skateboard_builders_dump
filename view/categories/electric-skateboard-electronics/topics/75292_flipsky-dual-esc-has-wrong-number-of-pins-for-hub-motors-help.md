# Flipsky Dual ESC has wrong number of pins for hub motors. Help!

### Replies: 38 Views: 1239

## \#1 Posted by: tkc Posted at: 2018-11-20T01:30:23.052Z Reads: 205

```
I am using a [Flipsky dual ESC](https://flipsky.net/collections/electronic-products/products/dual-fsesc4-12-100a) and  [WOWGO hub motors](https://wowgoboard.com/collections/new-theme/products/hub-motor-90mm) but one thing I noticed was the motor (hall?) sensors have 5 wires (red, yellow, blue, green, black). But the pins on the board are for 6, or for 4, or for 7. So... how the hell do I get this working with the VESC tool?

![IMG_4532|375x500](upload://xKQwm694XlSUHIczAWe6MKy7Q4t.jpeg)
```

---
## \#2 Posted by: nuttyjeff Posted at: 2018-11-20T01:53:22.721Z Reads: 192

```
It's simply because the hall sensors on the VESC have a temp pin for sensors with a temperature sensor. The 6 pins are temp, 5v, H1, H2, H3 and GND not in any psrticular order. You have to figure out which pins go where and plug it in sccordingly. The red and black wires from your motors are usually 5V and GND, while the remaining 3 wires are your hall sensor wires. It doesnt matter which order the hall sensor wires get plugged in to H1, H2, H3 of the VESC, as long as each one gets plugged into one of the 3.

They have also have a manual on their website..

![Screenshot_20181120_095558|525x500](upload://q8iks7UFRxpxFCpSYkZvxAmbnnN.jpeg)
```

---
## \#3 Posted by: tkc Posted at: 2018-11-20T01:58:46.896Z Reads: 179

```
Ok thanks for that. Makes sense. And yeah, I guess I could have checked their website. They didn't send any instructions with their product so I only had 1 youtube video to watch.
```

---
## \#4 Posted by: tkc Posted at: 2018-11-20T02:03:52.185Z Reads: 177

```
Sucks that the temp sensor is in the middle there and the positive and negative are on the outside. I'm going to have to figure out how to get the right wires in the right places.
```

---
## \#5 Posted by: nuttyjeff Posted at: 2018-11-20T02:07:04.349Z Reads: 178

```
They usually send a printed copy of that picture with their product. Guess they forgot to pack it with yours.

You could buy a *6pin connector and reconnect the pins. Fairly easy to do.
```

---
## \#6 Posted by: tkc Posted at: 2018-11-20T02:08:38.393Z Reads: 172

```
You mean a 6-pin connector, right? I can give it a try.
```

---
## \#7 Posted by: Sn4pz Posted at: 2018-11-20T02:37:02.732Z Reads: 165

```
Can you show me the sensors on your hubs? the photo is too small in the website. Im about to solder the sensor wires to my ownboard ESC that I have, with koowheel hubs....

cant wait to see your final product. are you going to put more power into them than the ownboard esc?
```

---
## \#8 Posted by: tkc Posted at: 2018-11-20T03:55:45.389Z Reads: 154

```
![IMG_4457|375x500](upload://oKobdU6Cu96D3efHxtLwWpJUcaG.jpeg) 

This is what comes off one of the motors
```

---
## \#9 Posted by: LEE Posted at: 2018-11-20T10:43:49.405Z Reads: 131

```
It is necessary to make it 6 pin with a gap between red and yellow.
Sometimes there is a 5 pin motor with no temperature sensor.
Wowgo's motor is one of them.
The motor sensor connector of the VESC is always 6 pins.
Next to red 5V is a temperature sensor.
Motor sensor cable 5 pins and 6 pins, the difference is whether or not there is a temperature sensor.
```

---
## \#10 Posted by: tkc Posted at: 2018-11-21T01:31:52.616Z Reads: 125

```
Ok so I made it 6-pin by soldering. I connected like so:

Red to red
Black to black
Yellow to yellow
Green to green
White to white
Orange to blue

However, the VESC tool is not picking up on the hall sensors still! What am I doing wrong? Pictures attached. 


![image|375x500](upload://wFf0bjGhim6B93tjIH2Z9f9sKLG.jpeg) 
![image|375x500](upload://lPkRZKwObyKvObmC8QhG6iKhkYb.jpeg)
![48%20PM|689x438](upload://bLvs1owWx91Y3iQDno85MWLELDm.png)
```

---
## \#11 Posted by: tkc Posted at: 2018-11-21T01:41:34.888Z Reads: 111

```
Here is a [video](https://youtu.be/LSL1-rDBez4) of what is happening and why I want to get the sensors working. What gives!?
```

---
## \#12 Posted by: dareno Posted at: 2018-11-21T04:47:47.638Z Reads: 105

```
I am a little confused my friend,  to reiterate.  The hubs have 5 cables and the vesc has 6 pins.  You know the pin out of the vesc but don't know the pin out on the motor.  How then have you made 6 solder joints?  Sounds to me like you have a hall sensor in the temp sensor pin on the vesc. Sounds like you need to know the exact function of the motor cabling.
@skateborad can you help this guy with some sensor info?
```

---
## \#13 Posted by: nuttyjeff Posted at: 2018-11-21T04:55:20.710Z Reads: 101

```
Magic! Hahaha.
```

---
## \#14 Posted by: tkc Posted at: 2018-11-21T05:00:46.819Z Reads: 101

```
The motors have 5 wires and a white wire that isn’t used. I went ahead and soldered that into the 6 wire setup I have so that white wire goes into the temp slot. But I know for sure (and you can see based on pictures) I wired them correctly.
```

---
## \#15 Posted by: tkc Posted at: 2018-11-21T05:03:42.041Z Reads: 102

```
I think my issues are similar to @DAddYE in:
[this thread](https://www.electric-skateboard.builders/t/105mm-airless-tire-hub-motor/65184/264?u=tkc)
```

---
## \#16 Posted by: dareno Posted at: 2018-11-21T05:33:27.956Z Reads: 104

```
It might be that the vesc is trying to detect a temp sensor without there being one on the motor.  Try disconnecting it and have another go.
```

---
## \#17 Posted by: Andy87 Posted at: 2018-11-21T05:49:57.758Z Reads: 99

```
you can check the faults in the terminal.
if one of the sensors is wrong or bad it should be written there.
look in termin ->actual faults after you made a sensor dedection.
```

---
## \#18 Posted by: LEE Posted at: 2018-11-21T06:05:57.377Z Reads: 98

```
![image|375x500](upload://bcqiUyRaq4adwpxJo3HI79Fn6oL.jpeg) 

This is the sensor wiring of my FLIPSKY hub motor.
There are 5wires from the motor.
There are also 5 wires to connect to VESC.
White wiring is not connected.
But the connector is 6 pins.
The temperature sensor is blank.
```

---
## \#19 Posted by: tkc Posted at: 2018-11-21T16:35:28.514Z Reads: 91

```
It looks like your green and yellow wires are reversed. Hmmm ok taking things apart to try it out!
```

---
## \#20 Posted by: LEE Posted at: 2018-11-21T16:48:38.011Z Reads: 96

```
Yellow, green, orange, these three can be replaced without problems.
The order does not matter.
From the left
① red · ② blank · ③④⑤ (yellow · orange · green) · ⑥ black
③, ④, ⑤. The order of this does not matter.
```

---
## \#21 Posted by: tkc Posted at: 2018-11-21T16:57:44.474Z Reads: 97

```
This is the second time I'm told the middle doesn't matter yet it's still not picking up the sensors. I have the red and black in place and I'm skipping the temp pin. What gives!?
```

---
## \#22 Posted by: tkc Posted at: 2018-11-21T17:09:04.918Z Reads: 97

```
Not sure I understand what you're saying. Did you mean debug console? Or you want me to type something in the terminal?

This is what I get in debug console:
    2018-11-21 12:00:55: Status: Bad FOC Hall Detection Result Received
    2018-11-21 12:00:55: Status: Bad FOC Hall Detection Result Received
    2018-11-21 12:07:14: Status: Bad FOC Hall Detection Result Received
    2018-11-21 12:07:14: Status: Bad FOC Hall Detection Result Received
```

---
## \#23 Posted by: Holyman92 Posted at: 2018-11-21T19:34:53.011Z Reads: 93

```
Did u not get the 5-6 cable? All my flipsky esc's came with the cable in the bag for the sensors and something else I forget, but look at the paper they included for the wiring and match it, I want to say the FS Esc's have their wiring flipped (I may be wrong tho) so the diagrams help


![15428290073541480630774|375x500](upload://r8fASgXkn0xWqOqMQ0HnK7bcooY.jpeg) 
This is thethe pinout for the single 6.6 fsesc

![15428290510671416081961|375x500](upload://txATrkchx5vfL5l5BMV7gE813uf.jpeg) 
This is the pinout for the dual 6.6 fsesc

On the 6.6 dual the sensor pin out is flipped so, one goes: 
black, yellow, green, orange, white, red

And the other goes:
Red, white, orange, green, yellow, black
```

---
## \#24 Posted by: tkc Posted at: 2018-11-21T19:47:04.864Z Reads: 80

```
I cut up some JST wires that they provided and soldered them together color matching (except for the orange to blue). I can now get one motor to register sensors but not the other. So weird.
```

---
## \#25 Posted by: Holyman92 Posted at: 2018-11-21T19:51:51.760Z Reads: 75

```
Did u make sure the 2nd one is opposite to the working  one?
```

---
## \#26 Posted by: tkc Posted at: 2018-11-21T22:23:57.547Z Reads: 77

```
According to the manual and the way the JST connector plugs in they both face the same way so negative is always on top.
```

---
## \#27 Posted by: Steven1 Posted at: 2018-11-21T22:54:28.502Z Reads: 75

```
That is incorrect, the Flipsky wiring diagram clearly shows that the left and right side hall sensor order is different. You are plugging them in wrong which is why you're getting the hall sensor fault. 

Here is the flipsky wiring diagram from their website:

![Flipsky%20wiring%20diagram|690x423](upload://5D800uLeMFoAgqLGZybBSSjU7jM.png)

Notice how one side V+ (red) is on top and on the other side GND (black) is on top.
```

---
## \#28 Posted by: Holyman92 Posted at: 2018-11-21T23:05:50.862Z Reads: 70

```
@Steven1 he's right i just looked up the diagram for his (4.2 dual) they are the same

![image|690x388](upload://kGbpaZtWXb8gzKklQQ01TYftdVQ.jpeg)
```

---
## \#29 Posted by: tkc Posted at: 2018-11-21T23:10:31.435Z Reads: 75

```
You are looking at a different ESC than the one I mentioned. Here is the manual for mine:
https://cdn.shopify.com/s/files/1/0011/4039/1996/files/Dual_FSESC4.20_100A_MANUAL_20181106.pdf.pdf?14152829648107869006
```

---
## \#30 Posted by: tkc Posted at: 2018-11-21T23:11:30.231Z Reads: 73

```
Plus the JST connector will only allow you to plug it into the board one way. Thus (hopefully) preventing someone from doing this. Stupid of Flipsky to have two ESC's doing different layouts though.
```

---
## \#31 Posted by: Andy87 Posted at: 2018-11-22T01:51:42.253Z Reads: 73

```
Nothing is flipped.
They both the same order.
Just one time the plug face to the right and the other time to the left.
```

---
## \#32 Posted by: Andy87 Posted at: 2018-11-22T01:54:06.394Z Reads: 71

```
I mean if you look up in the menu, there should be unter terminal I think be the option to show actual faults.
Was hoping to see there some more information,
I had once a bad result and checked there tha fault statistics. It said me the temp sensor is like -50 what means that my fault was with the temp sensor or the wiring of it.
```

---
## \#33 Posted by: Andy87 Posted at: 2018-11-22T02:01:32.140Z Reads: 67

```
Your wire order seem right according to the drawings.
From where you have the white one?
I thought the temp wire is missing and you have only 5 wires?
If no temp sensor than also don’t connect the white wire.
```

---
## \#34 Posted by: tkc Posted at: 2018-11-22T02:18:50.686Z Reads: 69

```
I think I know what’s happening. I finally got one to pick up on the sensors but not the other one. I went for a ride and at one point things got slow. I picked up the board and only one motor was spinning. I pushed in the connectors that come with the wheels that convert the cable type and got power again. I think that connector might have been loose. Will verify tomorrow!
```

---
## \#35 Posted by: Steven1 Posted at: 2018-11-22T07:28:37.913Z Reads: 65

```
I stand corrected. Thought we were talking bout the 6.6. If it's a lose connector it'll be a very easy fix :smile:
```

---
## \#36 Posted by: dareno Posted at: 2018-11-22T10:16:15.183Z Reads: 67

```
Round in circles here.  

[quote="Andy87, post:33, topic:75292"]
From where you have the wgute one?
I thought the temp wire is missing and you have only 5 wires?
If no temp sensor than also don’t connect the white wire.
[/quote]

[quote="dareno, post:16, topic:75292, full:true"]
It might be that the vesc is trying to detect a temp sensor without there being one on the motor. Try disconnecting it and have another go.
[/quote]
```

---
## \#37 Posted by: tkc Posted at: 2018-11-22T17:20:02.965Z Reads: 61

```
I did that. Made no difference.
```

---
## \#38 Posted by: skateborad Posted at: 2018-12-01T10:36:26.878Z Reads: 59

```
Let me check the topic.:rofl:
```

---
