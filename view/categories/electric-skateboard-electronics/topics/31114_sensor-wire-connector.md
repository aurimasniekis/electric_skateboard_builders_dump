# Sensor wire connector

### Replies: 37 Views: 1944

## \#1 Posted by: ikjahaa Posted at: 2017-08-20T18:20:42.379Z Reads: 272

```
Next to our bullet connectors for the motor phase wires we still use the ugly 6-pin connector for the sensor wires.

That's the reason why I'm looking for a different connector.
I'd like it to be small and clean.

I was thinking of:

* RJ-11 plug
The female connector of an RJ-11 tend to be pretty big. :confused:


* [6 pin 3.6mm jack (like on your phone)](https://www.alibaba.com/product-detail/6-pin-3-6mm-phone-jack_60682486720.html?spm=a2700.7724857.main07.1.2bd13975UpoLQ0&s=p)
Issue here is, i dont want 1000 units lmao.
Also cant find the male connector :confused:

Any ideas ?
```

---
## \#2 Posted by: deucesdown Posted at: 2017-08-21T01:56:47.542Z Reads: 250

```
Microusb? I've gotten small quantities of connectors from amazon and ebay. Good for many cycles, but not sure how robust against vibration.

https://never-stop-building-blog-production.s3.amazonaws.com/pictures/wiring-micro-usb-pinout/usb-microb-plug-connector-4.jpg

MPX? Six pins, robust, high current. Looks like there are panel mounts options.

https://www.yuki-model.de/cn_en/prodpic/Mounting-frame-gold-connector-YUKI-MODEL-compatible-with-MULTIPLEX-MPX-600207_b_0.JPG
```

---
## \#3 Posted by: deucesdown Posted at: 2017-08-21T02:04:52.530Z Reads: 234

```
I'm always thinking about connectors... I'll probably use these for the extension, when I get around to doing sensored.

https://cdn-shop.adafruit.com/1200x900/1664-03.jpg
```

---
## \#4 Posted by: scepterr Posted at: 2017-08-21T02:09:48.169Z Reads: 227

```
Not to go off topic but there's this alternative to the bullet connector, MT60 
<img src="/uploads/db1493/original/3X/9/3/93564e71d78b26fbb38a314634c1f2f3339c5c34.jpg" width="125" height="125"><img src="/uploads/db1493/original/3X/2/4/24b9a76a83a30ab96d202283c9a3b8acbe7a2ef5.jpg" width="125" height="125"><img src="/uploads/db1493/original/3X/b/f/bffb78e4b777f47a0587de31507b5cb87bb57d35.jpg" width="125" height="125">
There's also this waterproof 9 pin for phase and sensor wires, best for low amperage motors <img src="/uploads/db1493/original/3X/6/b/6b8b65f0219f8b6e54370789c6520671ec706049.jpg" width="250" height="250">
https://bmsbattery.com/ebike-parts/439-a-pair-of-9pin-waterproof-male-female-connector-cable-for-motor-parts.html
```

---
## \#5 Posted by: ikjahaa Posted at: 2017-08-21T06:25:13.036Z Reads: 203

```
I stil prefer the bullet connectors, reason why is because i think those connection points are way to close to each other. Especially for +40amps draw to your motor
```

---
## \#6 Posted by: scepterr Posted at: 2017-08-21T06:29:27.050Z Reads: 201

```
It's a 60A connector, and heatshrink the soldered connections
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-21T06:40:16.969Z Reads: 199

```
voltage would be what you need to worry about for distance of connections. That said, there's plenty of space between them for 60v~, not to mention each lead is insulated by plastic.
```

---
## \#8 Posted by: ikjahaa Posted at: 2017-08-21T07:03:33.148Z Reads: 200

```
Aha, and here u was thinking it was amps. Haha.
Hmm yea in that case.... 😉


Still in search for a good half sensor connector though
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-21T07:07:26.874Z Reads: 195

```
i'm still not sure what you mean exactly. the JST-PH connector is fairly small, are you worried about the individual cables? You could put them in some cable braid or another wrapping, looks pretty good!
```

---
## \#10 Posted by: ikjahaa Posted at: 2017-08-21T07:12:12.417Z Reads: 193

```
Yes the hall sensor wire connector. I still find it to be to big. I found a nice print on thingyverse which acts as a riser and a motor bullet connector holder thingy. Everything fits fairly nice, only the hal sensor connector is yea euhm too long.
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-21T07:13:27.230Z Reads: 182

```
hm i'm still not seeing the benefit, it's all inside your board anyway. With your proposition it seems like putting a converter in there would make it even more unsightly.
```

---
## \#12 Posted by: ikjahaa Posted at: 2017-08-21T07:15:42.232Z Reads: 188

```
No the bullet connector and sensor connector are the only wires outside my board..
```

---
## \#13 Posted by: Jinra Posted at: 2017-08-21T07:17:42.151Z Reads: 189

```
Do you have a pic? This is mine..

You can see that the phase wires are outside, but my sensor plug is inside the enclosure, your's is outside?
<img src="/uploads/db1493/original/3X/8/8/88d884c49a4cafbdce5b40a5d575bee9af9e7723.jpg" width="666" height="500">
```

---
## \#14 Posted by: ikjahaa Posted at: 2017-08-21T07:19:59.694Z Reads: 183

```
I see. 
Well I'm going to run my cabling through my deck. So it will be need to be plugged into the deck, which will be connected to my vesc
```

---
## \#15 Posted by: Jinra Posted at: 2017-08-21T07:24:10.986Z Reads: 174

```
Ah gotcha, sort of like LHB's builds, if I'm thinking about that right.
```

---
## \#16 Posted by: BoostedBuilder Posted at: 2017-08-21T07:26:37.513Z Reads: 181

```
So would you say that this connector is good for 42V and 60A??
```

---
## \#17 Posted by: Jinra Posted at: 2017-08-21T07:27:16.700Z Reads: 177

```
Yea I'm sure it's fine, the raptor 2 uses even smaller connectors.
```

---
## \#18 Posted by: krloz Posted at: 2017-08-21T07:30:10.346Z Reads: 183

```
[quote="ikjahaa, post:1, topic:31114"]
6 pin 3.6mm jack (like on your phone)
Issue here is, i dont want 1000 units lmao.
Also cant find the male connector
[/quote]

Those "6 pin" connectors only have 4 connections.  Ground, left and right audio and video the other two are for Jack sensing and switching off loudspeakers when something is plugged.  That's why you can't find a 6 pin male.  They don't exist.  They are the 4 pin male kind.  And that's one of the reasons why you can't use them for halls.
The other reason is. Never plug something that carries power through a connector that slides through other connections until it is completely plugged in.  Notice how the connectors we use always have pins one next to another and not in the same row?  That noise you sometimes get while slowly plugging in your headphones would equal a short in the 5v bus of the vesc
```

---
## \#19 Posted by: scepterr Posted at: 2017-08-21T07:31:07.281Z Reads: 174

```
@Jinra I think @BoostedBuilder is referring to the 9 pin. I strongly doubt it can handle 42V 60A, I wouldn't pump more than 1000watts cont through that cable and even then for 20-30secs tops
```

---
## \#20 Posted by: Jinra Posted at: 2017-08-21T07:32:15.560Z Reads: 175

```
Oh yea, i was talking about the MT60
```

---
## \#21 Posted by: ikjahaa Posted at: 2017-08-21T17:34:14.847Z Reads: 147

```
Not talking about the phase wires, I'm looking for a connectorbto be used for the hal sensor wires. 
Even the wires coming out of the motor can't handle 60a, or am I mistaking ?
```

---
## \#22 Posted by: ikjahaa Posted at: 2017-08-21T17:35:59.998Z Reads: 144

```
Yes, I get it... but the plug would only be connected when the board is off. 
But then again, what if the connector gets wanked out while riding .. hmmm... good point !

I'm seriously thinking of going sensorLESS hahaha
```

---
## \#23 Posted by: longhairedboy Posted at: 2017-08-21T17:36:23.214Z Reads: 146

```
That's what Evolve uses in thier boards.
```

---
## \#24 Posted by: scepterr Posted at: 2017-08-21T17:37:35.694Z Reads: 153

```
The MT60 or 9 pin?
```

---
## \#25 Posted by: longhairedboy Posted at: 2017-08-21T17:38:44.707Z Reads: 152

```
i want a small version of the Mini DIN used on the old PS2 keyboards. Its round and has 6 pins. but those don't lock in place with any real amount of friction. 

I'm on the hunt for this too and have been for a little while. I'd really like to be able to order my motors with a round connector and an adapter for vesc type escs. so i'll post anything i find.
```

---
## \#26 Posted by: ikjahaa Posted at: 2017-08-21T17:42:01.220Z Reads: 150

```
Yeahh hahaha 
I was even think to design a connector myself lmao
```

---
## \#27 Posted by: longhairedboy Posted at: 2017-08-21T17:48:10.352Z Reads: 149

```
do it! i'll buy them.
```

---
## \#28 Posted by: scepterr Posted at: 2017-08-21T18:06:20.151Z Reads: 152

```
There's these, but I think a bit bulky
<img src="/uploads/db1493/original/3X/6/1/61894cfc6d274ae44cb9cb4a5a357661c75ddbe9.jpg" width="281" height="500">
```

---
## \#29 Posted by: longhairedboy Posted at: 2017-08-21T18:09:23.799Z Reads: 138

```
i think i'm going to check them out. I haven't seen those yet.
```

---
## \#30 Posted by: deucesdown Posted at: 2017-08-21T18:54:05.332Z Reads: 137

```
I'm still liking the options i showed. Female micro-usb here, it's not too bad to solder.

https://ae01.alicdn.com/kf/HTB1ix23OVXXXXaIXpXXq6xXFXXXD/50Pcs-Micro-font-b-USB-b-font-Type-B-5Pin-Female-Horns-Reverse-SMT-Socket-PCB.jpg

Pretty small, if using these with heatshrink. And microusb is surprisingly robust, rated for 10,000 insertions, and has some retention built in. I'd still heatshrink the whole connection if using for sense wires...

You can also get them with housings, at least the male end

http://echista.ir/1232-thickbox_default/%D9%81%DB%8C%D8%B4-%D9%86%D8%B1%DB%8C-microusb-%D8%B3%D8%B1-%D8%B3%DB%8C%D9%85.jpg

MPX is about the size of XT60.

https://s-media-cache-ak0.pinimg.com/736x/d5/62/3f/d5623ff44b9aaddfe788520fe1376fc6--stecker.jpg
```

---
## \#31 Posted by: scepterr Posted at: 2017-08-21T18:59:14.069Z Reads: 136

```
If you wanna go usb, use a breakout board, sturdier
I use these when replacing microusb in noname random devices ;)
Also I think it would be possible to find a breakout board that matches the pin pitch of the PCB so you can just solder the breakout directly to PCB with pins or leads
<img src="/uploads/db1493/original/3X/a/9/a9a76a5875c3a24f08e38ad1a6a0394756f9d9ca.jpg" width="281" height="500">
```

---
## \#32 Posted by: ikjahaa Posted at: 2017-08-21T19:32:01.050Z Reads: 133

```
I'm wondering, howmuch Volt and Amps do these connectors need to be able to hold ?
```

---
## \#33 Posted by: scepterr Posted at: 2017-08-21T21:36:32.972Z Reads: 136

```
Quick mockup
<img src="/uploads/db1493/original/3X/1/6/168fd3062e2d69998d425192c443598c30e679c5.jpg" width="375" height="499"><img src="/uploads/db1493/original/3X/c/d/cd07f9c89543ff533cbfba396a4af5299b4da194.jpg" width="375" height="499">
Also could use usb-c breakout and itll be reversible
```

---
## \#34 Posted by: Jsk8 Posted at: 2018-10-22T22:07:58.734Z Reads: 81

```
![image|281x500](upload://yaODi5XqXokIZ2kyvh4V8Y15Gc2.jpeg) 


My motors came like this and they dont have a connector for the hall sensor wires and so there isnt a way for me to plug my hall sensor wires into the esc
Does anyone know how i can connect it or where i can get hall sensor connectors
```

---
## \#35 Posted by: ducktaperules Posted at: 2019-05-17T13:58:08.733Z Reads: 50

```
anyone ever find a good solution for this?
```

---
## \#36 Posted by: Jinra Posted at: 2019-05-17T15:20:22.318Z Reads: 48

```
This would work for most boards. Probably don't want to use it for very high powered boards though.

https://www.ebay.com/itm/Motor-cable-with-9-pin-waterproof-connector-male-and-female-for-motor/323631524506?hash=item4b59f12a9a:g:KXAAAOSwORRbejUR
```

---
## \#37 Posted by: Zertax Posted at: 2019-06-30T11:42:07.997Z Reads: 37

```
How bad would it be to get water in my sensor wire connection? Will it destroy something?
```

---
