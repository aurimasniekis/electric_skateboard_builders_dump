# Need help with electronics

### Replies: 73 Views: 2651

## \#1 Posted by: pcbacon Posted at: 2016-08-09T03:46:10.796Z Reads: 128

```
so I have recreated this but it doesnt seem to work when i put in the xt90  <img src="/uploads/db1493/original/2X/e/e4086365a6e9c08723fc31f200b9c65f3a1d1f51.PNG" width="478" height="500">
Here is what ive done <img src="/uploads/db1493/original/2X/c/cf01597af3137c1c3bfb176f22e3a8398499b5dc.JPG" width="375" height="500">
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-09T04:20:21.171Z Reads: 123

```
* Do you have a multi-meter? I would check voltages at every point to make sure there's no breaks anywhere.
* I'm assuming the top port on the right side is charging and the bottom is the cutoff switch? 
* Is the cut of switch an anti spark plug, or a button? 
* Did you make sure you plugged it in/switched it on? 
* Can we get a picture with the batteries in view?
```

---
## \#3 Posted by: pcbacon Posted at: 2016-08-09T04:42:32.455Z Reads: 120

```
I have used the multimeter everything is connected but when I use it over the xt90 no voltage goes through it and 44 volts going through the xt60 (charging port). but when I connect the two balance ports of the batteries together with my adapter. The xt90 connector has 22.2 V and same with the xt60 (charging port). But it still does not turn on. My xt90 anti spark hasn't arrived yet. and here are some more photos <img src="/uploads/db1493/original/2X/1/12fdbab0494c458c989db0403d3580f9dfb38633.JPG" width="666" height="500"> <img src="/uploads/db1493/original/2X/9/967757f5dc115ce0d0d48f3d548f3a544c67fda3.JPG" width="375" height="500"><img src="/uploads/db1493/original/2X/2/28f62b8ff9914b6fca3f0a1884e5e78dc044cdc3.JPG" width="375" height="500"><img src="/uploads/db1493/original/2X/0/0d684fa494b760b546aa2b35078be96ed808ed56.JPG" width="375" height="500">
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-09T04:49:13.468Z Reads: 102

```
Well there's your problem You have 1 pair of wires labeld '+' on the xt60 but its actually a + and - from 1 pack. Same goes for the one labled '-'. If you take a look at the diagram you can see that they have 2 of the same polarity wire going in parallel to the respective destinations.

Your VESC right now is receiving 2 positive connections.
```

---
## \#5 Posted by: pcbacon Posted at: 2016-08-09T04:53:38.819Z Reads: 98

```
oh no sorry don't worry about my labeling but you can see the black wire from the Esc connects to the black wire on the battery in the third photo
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-09T04:56:26.110Z Reads: 99

```
Ah I see, it was hidden behind the other wire. Either way, You're circuit is not complete because the two packs don't connect in any way. Let me see if I can draft up a fix for you.
```

---
## \#7 Posted by: pcbacon Posted at: 2016-08-09T04:57:29.099Z Reads: 97

```
but the guy that made that schematic said his worked fine before and had no problems
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-09T04:57:56.491Z Reads: 96

```
Yea, but your setup isn't hooked up according to the diagram, give me a minute.
```

---
## \#9 Posted by: makevoid Posted at: 2016-08-09T04:58:01.179Z Reads: 92

```
your wires are not connected the same way as the pictures shows, yours go from one plug to the other in series, I guess that if you close the circuit on the poles of the black plug you will be able to read the voltage correctly on the xt90, also I don't think you can keep the parallel circuit (charging circuit) close while using the main one (discharging circuit / series) , but I may be wrong
```

---
## \#10 Posted by: pcbacon Posted at: 2016-08-09T04:59:31.212Z Reads: 90

```
I think my wires are connected fine i just switch the xt60 and the xt90
```

---
## \#11 Posted by: Jinra Posted at: 2016-08-09T05:00:18.572Z Reads: 92

```
I think this should do it. Switch the wires as shown. Black wire (circled green) goes to where the Red wire (circled red) should be, and vice versa.

<img src="/uploads/db1493/original/2X/5/57b5b3c6174bef8eec671d599908c79eaffd52a0.jpg" width="666" height="500">
```

---
## \#12 Posted by: pcbacon Posted at: 2016-08-09T05:01:31.247Z Reads: 86

```
will that still keep it in parallel?
```

---
## \#13 Posted by: makevoid Posted at: 2016-08-09T05:02:20.964Z Reads: 84

```
see this diagram (edit: this is for 12s)

http://www.electric-skateboard.builders/uploads/db1493/original/2X/d/d1926c2991d7cb6b0e44273dcd8785f5dd8f8b09.JPG

the one that you're using doesn't really shows the connections, then you can join the xt60s and the balance leads in parallel
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-09T05:02:46.286Z Reads: 79

```
Yes, though 1 more change you need to do is short the connections on the XT60, it'd be easier if you just scrapped the XT60's and soldered the wires together instead.
```

---
## \#15 Posted by: pcbacon Posted at: 2016-08-09T05:03:49.102Z Reads: 78

```
are you sure because i want to be able to remove them just in case and not have to solder them out
```

---
## \#16 Posted by: pcbacon Posted at: 2016-08-09T05:04:31.756Z Reads: 80

```
i see but that is in series
```

---
## \#17 Posted by: Jinra Posted at: 2016-08-09T05:05:49.756Z Reads: 83

```
Yea, I'm pretty sure, but like I said the XT60's have to either be shorted, or removed altogether.
```

---
## \#18 Posted by: makevoid Posted at: 2016-08-09T05:06:23.793Z Reads: 80

```
oh you want 6S in parallel? I thought you wanted 12S, than that's easier
```

---
## \#19 Posted by: pcbacon Posted at: 2016-08-09T05:06:56.238Z Reads: 78

```
okay I will do this change tomorrow and I will let you know how it goes. Thank you so much btw
```

---
## \#20 Posted by: pcbacon Posted at: 2016-08-09T05:13:20.581Z Reads: 79

```
thank you for your help anyways
```

---
## \#21 Posted by: Jinra Posted at: 2016-08-09T05:14:40.408Z Reads: 76

```
no problem. it's important to understand how everything's hooked up, so look over the fix and try to understand it. Let me know if you have any questions.
```

---
## \#22 Posted by: makevoid Posted at: 2016-08-09T05:21:32.562Z Reads: 76

```
here's a simpler diagram of what you want to do, first connect the batteries in parallel, then after you've done that connect everything else

simpler:

https://docs.google.com/presentation/d/1Z8upFzhj7q6ZXoV4I6j_G-2-aGsM4aHqR9BJGmnU2Gc/edit?usp=sharing

using plugs:


https://docs.google.com/presentation/d/1NvyL7uattnfvb36Qj956t7bo1HUVgBbv5pZe2l-WKaE/edit?usp=sharing

the base idea is you think as your parallel battery as one big battery and then you can charge it directly and have a xt90 as switch as the last bit in your circuit
```

---
## \#23 Posted by: Jinra Posted at: 2016-08-09T05:23:59.251Z Reads: 67

```
Yep like that. That should how it's setup if he does my suggestion, the only difference is the "loop key", in this case the power switch, is on the positive lead instead.
```

---
## \#24 Posted by: makevoid Posted at: 2016-08-09T05:30:01.076Z Reads: 68

```
I think they will short like that because you can see there's another wire at the back that will close the +/- circuit

<img src="/uploads/db1493/original/2X/5/5d9d2d0babc96d0ac654dd1998af901c7c712cd3.jpg" width="674" height="500">
```

---
## \#25 Posted by: Jinra Posted at: 2016-08-09T05:31:19.007Z Reads: 64

```
I'm not sure what you mean, why would that short? It should be pretty much the same as the diagram you posted.
```

---
## \#26 Posted by: makevoid Posted at: 2016-08-09T05:33:48.461Z Reads: 65

```
[quote="Jinra, post:17, topic:7343"]
or removed altogether.
[/quote]

You are right when you say it should be removed, otherwise if you close the circuit at the xt60  it will short + and - of the same battery
```

---
## \#27 Posted by: Jinra Posted at: 2016-08-09T05:37:43.398Z Reads: 65

```
Still not following you. If he swaps the cables like I pictured, and shorts each of the + and - labeled xt60 connectors, it'll create a parallel connection for the two packs as you picture. Shorting the connector is essentially the same as soldering the two cables together.

@pcbacon - One more change now that i look at it again is to swap the two cables on the charging port as well. Positive leads should go to the flat side of the xt60 while negative goes to the angled side.
```

---
## \#28 Posted by: makevoid Posted at: 2016-08-09T05:38:32.490Z Reads: 63

```
oh, no sorry, my mistake, **it will work,** I inverted xt60 with xt90 in my mind lol :D  because I have yellow xt90 and I've seen black xt60 recently lol

you're right @jinra it will work, sorry for the confusion
```

---
## \#29 Posted by: Namasaki Posted at: 2016-08-09T05:49:18.710Z Reads: 61

```
Easiest way to avoid confusion is to connect the 2 batteries in parallel first using a Y connector and then you will have 1 black and 1 red wire coming from the battery packs. run the black and red to the charge port and from the charge port run the black straight to the esc and the red from the charge port to the anti spark jumper and from that to the esc.
```

---
## \#30 Posted by: pcbacon Posted at: 2016-08-09T06:21:40.700Z Reads: 57

```
Still didn't work I just did it what you said
```

---
## \#31 Posted by: pcbacon Posted at: 2016-08-09T06:26:53.297Z Reads: 62

```
this was before the change and after<img src="/uploads/db1493/original/2X/2/21d0ac4b19dd28fc9e57fcd1b9d179109a053354.jpg" width="666" height="500">
After
<img src="/uploads/db1493/original/2X/0/0583747a5949b17a93430104336660eb17c6acc3.jpg" width="666" height="500">
so we technically changed nothing in the two
```

---
## \#32 Posted by: Jinra Posted at: 2016-08-09T06:31:48.548Z Reads: 55

```
Did you short the XT60 or remove it and solder directly as well? That was also very important.
```

---
## \#33 Posted by: pcbacon Posted at: 2016-08-09T06:33:03.889Z Reads: 56

```
but it doesn't change anything see ^
```

---
## \#34 Posted by: Jinra Posted at: 2016-08-09T06:34:54.228Z Reads: 54

```
But it does change.. Before you had it hooked up in series on an incomplete circuit. After is parallel. Like I said you need to short the XT60s on the + and - marked leads or else it's still an incomplete circuit.
```

---
## \#35 Posted by: pcbacon Posted at: 2016-08-09T06:36:32.382Z Reads: 53

```
so i have to short the xt60 but in the schematic he didnt have to short the xt 60
```

---
## \#36 Posted by: Jinra Posted at: 2016-08-09T06:37:22.515Z Reads: 55

```
That's because in the schematic they didn't have XT60's where you have them. They just soldered the wires together to create a parallel connection. Either option works, since you already have the XT60's there I thought it might be easier for you to short the cables.
```

---
## \#37 Posted by: pcbacon Posted at: 2016-08-09T06:41:00.635Z Reads: 53

```
okay so if it wouldnt be to much trouble good you draw it out for me?
```

---
## \#38 Posted by: Jinra Posted at: 2016-08-09T06:43:41.674Z Reads: 55

```
Short the wires where the blue is **after** you swap the red/black cables.
<img src="/uploads/db1493/original/2X/4/45f8f4cf01468cd76e63cf650607e2add94a086f.jpg" width="666" height="500">
```

---
## \#39 Posted by: Titoxd10001 Posted at: 2016-08-09T06:46:40.702Z Reads: 51

```
Are you using a loop key?
```

---
## \#40 Posted by: pcbacon Posted at: 2016-08-09T06:50:56.469Z Reads: 50

```
yes i am ueing a loop key for the xt90
```

---
## \#41 Posted by: pcbacon Posted at: 2016-08-09T06:51:36.575Z Reads: 45

```
okay so the two black and two red will be connected as one the will split again?
```

---
## \#42 Posted by: Jinra Posted at: 2016-08-09T06:52:40.706Z Reads: 46

```
Yep! that's a parallel connection. See the original schematic you posted, it's the same way. 2 black and 2 reds join together and then split.
```

---
## \#43 Posted by: pcbacon Posted at: 2016-08-09T06:55:47.074Z Reads: 46

```
oh okay I must have miss read it. I am definitely doing tomorrow dont have time tonight
```

---
## \#44 Posted by: pcbacon Posted at: 2016-08-09T23:12:50.460Z Reads: 39

```
I have done that and still does not work i connected the red and red, black and black then hooked it all up still the same result
```

---
## \#45 Posted by: Jinra Posted at: 2016-08-09T23:14:11.363Z Reads: 38

```
You shorted the XT60's? take a multimeter and measure the leads going to the VESC.
```

---
## \#46 Posted by: pcbacon Posted at: 2016-08-09T23:23:25.935Z Reads: 35

```
do I have to short the xt60? the VESC is getting 22.4V. i noticed that the VESC is getting a little warm
```

---
## \#47 Posted by: pcbacon Posted at: 2016-08-09T23:23:58.393Z Reads: 35

```
the VESC was working fine when i tested it with just one lipo tho
```

---
## \#48 Posted by: Jinra Posted at: 2016-08-09T23:25:01.005Z Reads: 35

```
Wait the VESC is powered? So what's not working?
```

---
## \#49 Posted by: pcbacon Posted at: 2016-08-09T23:26:38.589Z Reads: 35

```
it appears to be powered but my receiver for my remote doesn't light up when i tested it out before with one lipo
```

---
## \#50 Posted by: Jinra Posted at: 2016-08-09T23:28:37.684Z Reads: 37

```
I'm unclear as to what you have done and what's working/not working for you. Did you short the blue areas like I mentioned last night? If so you should have a parallel connection between both packs.

It sounds like you have a receiver issue more than a cabling issue now right?
```

---
## \#51 Posted by: pcbacon Posted at: 2016-08-09T23:29:42.504Z Reads: 39

```
should I try testing the VESC receiver cable with a multimeter?
```

---
## \#52 Posted by: Jinra Posted at: 2016-08-09T23:30:15.981Z Reads: 39

```
couldn't hurt, just probe the red and black cable on the receiver and you should get 5v.
```

---
## \#53 Posted by: pcbacon Posted at: 2016-08-09T23:39:46.161Z Reads: 38

```
alright it works I think my receiver is dead i bought this one and was working but it seems it does not want to work anymore
http://www.electric-skateboard.builders/t/2-4ghz-nano-remote-in-stock-30-pcs-usa-50-free-priority-shipping-international-45-shipping/5017/201
```

---
## \#54 Posted by: Jinra Posted at: 2016-08-09T23:40:55.317Z Reads: 38

```
I have the same one and it works great for me. Please make sure you follow binding procedure and configure the min/max pulsewidth on the PPM tab.
```

---
## \#55 Posted by: pcbacon Posted at: 2016-08-09T23:41:30.210Z Reads: 37

```
how do i adjust the min/max pulsewidth when i cannot connect it
```

---
## \#56 Posted by: Jinra Posted at: 2016-08-09T23:41:58.852Z Reads: 40

```
Well the pre-requisite is to make sure it's bound. Have you try rebinding?
```

---
## \#57 Posted by: pcbacon Posted at: 2016-08-09T23:42:07.847Z Reads: 39

```
the receiver is very finicky i plug it in barley and it lights up then it goes off very strange
```

---
## \#58 Posted by: Jinra Posted at: 2016-08-09T23:42:48.021Z Reads: 39

```
maybe you have a break in the servo cable, try a different one?
```

---
## \#59 Posted by: pcbacon Posted at: 2016-08-09T23:55:00.394Z Reads: 39

```
okay, I have done some measuring the VESC servo cable gives out around 7V when not plugged in but when I plug it in the receiver it only gives out about 1V and no light on the receiver. any ideas?
```

---
## \#60 Posted by: Jinra Posted at: 2016-08-09T23:55:51.672Z Reads: 39

```
Sounds like a short somewhere, maybe the cable?
```

---
## \#61 Posted by: pcbacon Posted at: 2016-08-09T23:57:00.040Z Reads: 34

```
cable looks fine no bends
```

---
## \#62 Posted by: Jinra Posted at: 2016-08-09T23:57:51.153Z Reads: 40

```
Not sure if it's supposed to be outputting 7v in the first place as it should be 5v. I would try a new cable.
```

---
## \#63 Posted by: pcbacon Posted at: 2016-08-09T23:59:06.374Z Reads: 42

```
do I get a new cable I gotta desoldered it from the VESC then solder a new one on?
```

---
## \#64 Posted by: Jinra Posted at: 2016-08-10T00:00:07.435Z Reads: 43

```
It's soldered onto the VESC? usually it's a just a male servo cable that plugs into it. I guess if it's soldered, then yea that's what you would have to do to change it, but i'm not sure what the problem might be at this moment.
```

---
## \#65 Posted by: pcbacon Posted at: 2016-08-10T00:02:10.230Z Reads: 45

```
oh you mean just the end part of the cable? cut that part off? this is my VESC http://www.hobbyking.com/hobbyking/store/__30845__Hobby_King_80A_ESC_4A_SBEC_US_Warehouse_.html?strSearch=80a
```

---
## \#66 Posted by: Jinra Posted at: 2016-08-10T00:04:08.333Z Reads: 45

```
OH, I thought you had a VESC this whole time. You have a regular hobby ESC. Though, this doesn't change much. It might be the cable, it might not. I don't want to tell you to rip out the cables if it doesn't turn out to be that. You'll have to test the connection and various positions to see if you can get a reading.
```

---
## \#67 Posted by: pcbacon Posted at: 2016-08-10T00:06:46.896Z Reads: 43

```
what is a VESC what's the difference?
```

---
## \#68 Posted by: Jinra Posted at: 2016-08-10T00:08:10.390Z Reads: 41

```
it's a highly customizable ESC which a ton of people on this forum use. I use two of them myself. It's the only ESC I know with current control instead of duty cycle as well.
```

---
## \#69 Posted by: pcbacon Posted at: 2016-08-10T00:10:15.951Z Reads: 43

```
what one do you use and where do you buy it from? I'll get one for my next board
```

---
## \#70 Posted by: Jinra Posted at: 2016-08-10T00:11:55.428Z Reads: 44

```
ollinboardcompany.com Best VESCs in the business IMO.
```

---
## \#71 Posted by: fottaz Posted at: 2016-09-03T12:07:41.736Z Reads: 37

```
Hi, I have another problem. Testing the motor by BLCD and the motor works fine but when I push the Nano receiver trottle it doesn't work. No signal, I've done binding, i have both Red lights but the motor can't move
<img src="/uploads/db1493/original/2X/9/9bd21b570f8fc400d79e6826a7f790d2520db458.jpg" width="662" height="500">
```

---
## \#72 Posted by: makevoid Posted at: 2016-09-03T18:18:53.413Z Reads: 30

```
Did you configure the vesc PPM settings in BLDC tool?
```

---
## \#73 Posted by: fottaz Posted at: 2016-09-03T18:55:37.993Z Reads: 30

```
Thanks I've already solved it by configuring PPM settings this afternoon and I've just done my evening ride and I'm soooo happy now 😀👌
```

---
