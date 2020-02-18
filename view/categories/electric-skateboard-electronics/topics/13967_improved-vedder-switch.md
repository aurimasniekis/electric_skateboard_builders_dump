# Improved vedder switch

### Replies: 20 Views: 2330

## \#1 Posted by: DeathCookies Posted at: 2016-11-30T15:48:30.564Z Reads: 306

```
Hey there,
i am not experienced with creating a pcb but some of the community are.

Could someone modify the current [Vedder Switch 1.4](https://oshpark.com/shared_projects/XuqJkZzU) that we will be able to attach a LED direct to the PCB like the torqueboards switch?
```

---
## \#2 Posted by: lox897 Posted at: 2016-11-30T19:33:15.678Z Reads: 281

```
Led or led switch?
```

---
## \#3 Posted by: DeathCookies Posted at: 2016-12-01T07:50:30.304Z Reads: 258

```
LED switch ;)
```

---
## \#4 Posted by: DeathCookies Posted at: 2016-12-01T07:51:42.938Z Reads: 254

```
[quote="DeathCookies, post:1, topic:13967"]
like the torqueboards switch
[/quote]

diy-electric-skateboard-kits-parts/electric-skateboard-on-off-power-switch/
```

---
## \#5 Posted by: chipoi84 Posted at: 2016-12-01T07:56:01.567Z Reads: 231

```
Can't we already use a led switch the current version of Vedder antispark pcb? I am using a similar led switch as torqueboard with my vedder antispark board.
```

---
## \#6 Posted by: lox897 Posted at: 2016-12-01T08:12:58.898Z Reads: 225

```
Yeah I think you can
```

---
## \#7 Posted by: TarzanHBK Posted at: 2016-12-01T08:24:50.348Z Reads: 219

```
we need a wiring diagram and a what kind of switch you use if its possible.
```

---
## \#8 Posted by: lox897 Posted at: 2016-12-01T08:43:41.186Z Reads: 209

```
@chaka might be able to tell you. I reckon the middle is for the led and the two outer pads are for the switch
```

---
## \#9 Posted by: DeathCookies Posted at: 2016-12-01T21:21:35.603Z Reads: 192

```
Not really. The problem is that the LED wont shine bright enough if you only attach it to the current circuit Design...
```

---
## \#10 Posted by: 2-alex-2 Posted at: 2016-12-01T21:29:42.248Z Reads: 193

```
I use an led switch and I have just wired the led wires to the output of the switch so then the switch is pressed switching the vesc on same power is used to switch the led on.
```

---
## \#11 Posted by: chipoi84 Posted at: 2016-12-01T22:10:00.371Z Reads: 189

```
Did you use it with 10s batttery pack? The one I have seemed bright enough. <img src="/uploads/db1493/original/3X/3/8/3838b0402ab4265391e063cea73493b833fac31f.jpg" width="689" height="481">
<img src="/uploads/db1493/original/3X/5/b/5bbc11be3418b18402362a45292773cc30d22a59.jpg" width="690" height="481">
And this is how I wired my board with the led power switch. Coming from the led, the red wire is positive, and black is ground. The green wire is C (Closed). The white wire is NO (Normally Opened). The Blue wire is NC (Normally Closed). The red wire (Positive) has to be connected to the white wire (NO) either by soldering or just simply pushing its wire into the "NO" slot. The white wire (NO) is soldered to the slot directly below the In-Postive of the Vedder Anti-spark board. The green wire (C) is soldered into the middle slot. The blue wire (NC) is soldered into the slot above the In-Negative of anti-spark board. Lastly, the black wire (Negative) from the led is soldered into the Out-Negative of the anti-spark board. Hope that make sense...
```

---
## \#12 Posted by: DeathCookies Posted at: 2016-12-02T07:44:27.560Z Reads: 174

```
For me it did not work as expected when i have hold the cables against the pin. I did not solder it yet. For testing purpose....

Maybe i should just solder it on and report back ;) thanks for the help!
```

---
## \#13 Posted by: SeanHacker Posted at: 2017-01-19T18:16:18.775Z Reads: 155

```
So I saw this thread and got curious about getting the LED switch to work. I have no electrical and barely any soldering skills. I literally just got into the eboard scene 2 months ago. Totally new at all of this. 

I started my first build and I really want an LED switch. So I tested on this cheap little guy today that I bought a while back https://www.amazon.com/gp/product/B01D2S6ZPK/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1. I wired it up and it works. The led light is really dim though. But it does function correctly and turns on and off as it should and also lights up. But as I said, the light is really dim. I ordered this one yesterday and it's on the way https://www.amazon.com/gp/product/B00ZR7MMXO/ref=oh_aui_detailpage_o00_s00?ie=UTF8&psc=1

Do any of you know how to get the light to get as bright as it should? Does the positive need to go somewhere else to get ample power to the LED? Don't mind the wiring. Nothing is color coded for now while testing. Any help at all would be appreciated. 

Here's a pic and video. For the video, everything was soldered up. You can see the the instant I press the power button it flashes bright really quick and then when it's fully engaged it's back to being very dim. 

<img src="/uploads/db1493/original/3X/8/2/8274d99b9b90e791c71823aff0c3f8a40904fd93.jpg" width="388" height="500">

https://www.youtube.com/watch?edit=vd&v=pIRu6SX6Sa4

<img src="/uploads/db1493/original/3X/f/0/f02a1ae27e93f77ffd8c22ddf613ab79bdd80a12.jpg" width="483" height="500">
```

---
## \#14 Posted by: TarzanHBK Posted at: 2017-01-20T11:07:41.942Z Reads: 131

```
@DeathCookies is working on this
```

---
## \#15 Posted by: Maxid Posted at: 2017-01-20T11:11:01.861Z Reads: 134

```
You don't have it hooked up to a power source but just to the switch poles? :confused:
```

---
## \#16 Posted by: SeanHacker Posted at: 2017-01-20T15:39:58.554Z Reads: 132

```
To be honest... I don't know? I'm literally winging everything. :)
```

---
## \#17 Posted by: Maxid Posted at: 2017-01-20T15:44:44.747Z Reads: 130

```
You have to connect the GND and +12V of the switch to the main cable pads behind the mosfets, together with a suitable resistor in line so that you adjust your battery voltage to the 12V used by the switch's LED.
```

---
## \#18 Posted by: NAF Posted at: 2017-01-20T15:48:26.464Z Reads: 127

```
Which button is it ? can you post a link ?
```

---
## \#19 Posted by: SeanHacker Posted at: 2017-01-20T15:53:33.687Z Reads: 129

```
https://www.amazon.com/gp/product/B01D2S6ZPK/ref=oh_aui_detailpage_o03_s00?ie=UTF8&psc=1

I think my vedder switch went out now. After my first charge up with my new build I turned it on and the board wouldn't turn off. Now I can't even get a regular rocker switch to work. Ugh...
```

---
## \#20 Posted by: DeathCookies Posted at: 2017-01-20T17:29:43.794Z Reads: 125

```
If we dont want to change the design of the switch (by adding another trace(?) and a resistor) this would be the only solution atm:

Just attach the LED + and - to the PCB like this. But you need to add a 3k-4k (maybe 6.8k?)resistor in front of the LED + that you dont get the complete current of the battery.
<img src="/uploads/db1493/original/3X/9/2/9217ac836a4c6be701e7558bb4a3f0cf43def3c8.jpg" width="690" height="387">

@JdogAwesome did i understand you correctly?
```

---
