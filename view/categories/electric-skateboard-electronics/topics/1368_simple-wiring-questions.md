# Simple Wiring Questions

### Replies: 21 Views: 3554

## \#1 Posted by: Andrew Posted at: 2016-02-15T01:53:20.250Z Reads: 198

```
I believe i finally have all the parts needed to start assembling my board. First problem i encounter is the actual wiring which i have no knowledge of. I was wondering if i would need to solder the wiring between the motor/esc/batteries(for charging)  together or if there was a connector (prefered method) i could buy. 
<img src="/uploads/db1493/original/2X/7/75bcba9b25b704bf3729748ace0cd085d5e7f755.jpg" width="375" height="500">

<img src="/uploads/db1493/original/2X/a/a764fc129a88c6bb51f9c28491289087e773b91a.jpg" width="666" height="500">

Another off topic question: connecting the batteries to the charger: came with a bunch of wires but not sure if i can use any of them..
<img src="/uploads/db1493/original/2X/4/46dae3bfcbd45d63206e2e586858b82ad8e045c2.jpg" width="375" height="500">

Please inform me! Thank you
```

---
## \#2 Posted by: EnertionSupport Posted at: 2016-02-15T02:03:31.554Z Reads: 193

```
The motor wires can be connected in any order. If the motor is spinning the wrong direction, simply flip two of the wires an the motor will then start spinning the other way. 

For this reason, it is nice to have bullet connectors (matching your motor connectors) that will allow you to switch the wires and disconnect them at will. That said, you could just solder them after making sure your motor was spinning in the right direction. 

For the battery, I would recommend a connector. You really don't want to leave your battery connected to the ESC at all times if you don't have to. 

It looks like the two charging connectors that come with your charger are deans (the dark red two-pronged ones) and an xt60 (the yellow one). So if you just buy a pair of either deans, or xt60's for your battery and esc, then you'd already have the correct charging cable to go with that connector.
```

---
## \#3 Posted by: laurnts Posted at: 2016-02-15T02:06:04.706Z Reads: 189

```
use 5.5 or 4.x bullet connector from Hobbyking. So you can easily attach and detatch. It that takes so long for you and you can't wait any longer, you could use the cheap cable connector (for test only).
<img src='/uploads/db1493/original/2X/8/829d6aa8c1bbfae740caf2f8a345e6291030543d.jpg'>

They can do the job to test, but they don't handle the current you will be drawing when you ride on your board.
```

---
## \#4 Posted by: cmatson Posted at: 2016-02-15T02:39:14.887Z Reads: 177

```
The bullet connectors are great, but I wouldn't even bother with the cheapo testing connectors that Laurnts recommended.. just have bullet connectors for the 3 phase wires (that match the ones already on the motor) so you can switch any wires whenever you want.
```

---
## \#5 Posted by: laurnts Posted at: 2016-02-15T02:43:31.255Z Reads: 172

```
I Agree it's not a safe practice! Since I live in a remote place of online stores with BS shipping cost, getting 5.5 bullet connector is a though job. This does the job quite well for testing :D BUT NOT RECOMMENDED to ride with it.
```

---
## \#6 Posted by: Andrew Posted at: 2016-02-15T02:55:58.360Z Reads: 171

```
Correct me if im wrong. It seems like i need this to charge the batteries.
http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=43863

And these to connect the esc to the batteries and the motor.
http://www.hobbyking.com/mobile/viewproduct.asp?idproduct=2087

2 questions regarding the bullet connector above:
1. Do i need to solder the bullet connector to the wiring?
2. How do i know if the batteries have 4mm or 5.5 mm connectors?
```

---
## \#7 Posted by: Andrew Posted at: 2016-02-15T18:51:46.058Z Reads: 152

```
Hey laurnts have any idea?
```

---
## \#8 Posted by: barajabali Posted at: 2016-02-15T20:21:51.042Z Reads: 148

```
@Andrew  You should invest in a soldering iron.  You wont need to buy all these adapters, you can just solder on any connectors you want/have as long as it can handle the current. 
All these adapters are gonna get annoying to work with
```

---
## \#9 Posted by: lowGuido Posted at: 2016-02-15T23:57:01.268Z Reads: 144

```
those 5.5mm adapters are not what you need.
you need this:
http://www.ebay.com.au/itm/like/251593471762?limghlpsr=true&hlpht=true&ul_noapp=true&hlpv=2&chn=ps&lpid=107&ops=true&viphx=1

but @barajabali  is right, just get a soldering iron..
```

---
## \#10 Posted by: Andrew Posted at: 2016-02-16T00:10:44.493Z Reads: 141

```
I would rather use adaptors as it is my first build and id rather not mess around with soldering things just yet
```

---
## \#11 Posted by: Andrew Posted at: 2016-02-16T00:11:32.708Z Reads: 139

```
Yes that is what i need in order to charge my batteries but im intrested in an adaptor to hook up the esc to the the motor and batteries
```

---
## \#12 Posted by: lowGuido Posted at: 2016-02-16T05:44:37.799Z Reads: 131

```
You gotta solder. There is no way around it
```

---
## \#13 Posted by: Andrew Posted at: 2016-02-16T06:27:23.123Z Reads: 124

```
How can i tell if my wires a 4 or 5.5 mm?
```

---
## \#14 Posted by: lowGuido Posted at: 2016-02-16T07:09:07.328Z Reads: 125

```
They are 4mm

Edit. Not sure why this came out bold. It wasn't supposed to be.
```

---
## \#15 Posted by: JLabs Posted at: 2016-02-16T14:42:17.441Z Reads: 124

```
I personally use a three way switch to an external xt60 connector that allows for charge without removal of the battery.  As for the adapter, you have to solder connectors, it took me 3 tries and ruined two connectors to get a good connection I was happy with, just don't cut corners when it comes to wiring wires that are carrying 22.2v (in my case) Good luck and leave a reply if you need any help, I'd be glad to help!
```

---
## \#16 Posted by: Sinno Posted at: 2016-02-21T01:29:06.982Z Reads: 117

```
I'm pretty new to rc/arduino/electric skateboard/electronics, but barajabali is correct. You won't find many ready made connectors on line, because no one is buying them! Everyone makes their own. I would start with a soldering iron with a temperature control. Keep your sponge wet! You will in the end. Have fun.
```

---
## \#17 Posted by: Hummie Posted at: 2016-02-21T11:43:31.524Z Reads: 118

```
 
Clamp the plug/connector with anything that can hold it steady and won't melt , get it hot with the iron, feed solder into the connector reservoir, enough that the wire can be sub urged in it, put the tinned wire in it and continue heating till its sitting in a pool of liquid solder, don't move it till it cools. 

  Getting lead solder and a higher watt iron made a huge difference for me.  I don't know what temp it gets to but it does it fast and fast is good when soldering
```

---
## \#18 Posted by: Cloud_Gnash Posted at: 2016-11-05T20:53:02.418Z Reads: 73

```
So one of my bullet wires keeps getting disconnected from my VESC every mile or so. Does anyone have recommendations on how to secure it so this doesnt happen? I feel like a gum type substance would work well but i thought the forum may have some suggestions @EnertionSupport !
```

---
## \#19 Posted by: jak Posted at: 2016-11-10T23:09:00.714Z Reads: 66

```
what size bullets? if it is 5.5 you could try spreading out the prongs abit.
```

---
## \#20 Posted by: jmasta Posted at: 2016-11-11T00:12:19.108Z Reads: 65

```
[quote="Cloud_Gnash, post:18, topic:1368, full:true"]
So one of my bullet wires keeps getting disconnected from my VESC every mile or so. Does anyone have recommendations on how to secure it so this doesnt happen? I feel like a gum type substance would work well but i thought the forum may have some suggestions @EnertionSupport !
[/quote]

umm.... tape?

You may also want to reconsider your wiring layout. Maybe you can change it around to give your wires more slack and prevent them from getting pulled out?
```

---
## \#21 Posted by: SageTX Posted at: 2016-11-11T04:51:03.925Z Reads: 57

```
Heat shrink tube.  Doesn't get sticky, practically permanent until you want it off.  A quick slice and you're ready to change  whatever you need.
```

---
