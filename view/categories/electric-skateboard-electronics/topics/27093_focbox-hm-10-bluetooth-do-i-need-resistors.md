# FOCBOX + HM-10 Bluetooth do I need resistors?

### Replies: 15 Views: 3029

## \#1 Posted by: DavidBanner Posted at: 2017-07-08T21:29:27.707Z Reads: 313

```
Having looked through a few threads I noticed a couple of posts recommending using resistors on the RX pin of the HC-05
:
<img src="/uploads/db1493/original/3X/9/e/9e80748422066be079b2cdfb97242abf01e19970.jpg" width="640" height="498">

Do I need to use these resistors on the HM-10 I have? The RX/TX is marked as being 3.3V

or can I just connect like this?:
<img src="/uploads/db1493/original/3X/4/d/4d71ac56b74352c1983e832c91ca8b555bfe83d4.jpg" width="594" height="487">
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-07-08T22:17:24.935Z Reads: 292

```
You don't need the resistor, but you need two cross the RX and TX as @Ackmaniac explain.  

[quote="Ackmaniac, post:1, topic:20888"]
You need to connect the Bluetooth module this wayvia the 
5V Vesc to VCC Module
GND Vesc to GND Module
RX Vesc to TX Module
TX Vesc to RX Module
So you see that RX and TX needs to be crossed.
[/quote]
```

---
## \#3 Posted by: DavidBanner Posted at: 2017-07-08T22:42:47.832Z Reads: 285

```
thanks for the info  :)
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-08-17T00:52:45.748Z Reads: 249

```
Thank you for this!
```

---
## \#5 Posted by: SilentException Posted at: 2017-08-17T01:13:11.266Z Reads: 243

```
Umm, not sure about this. Two resistors act as a voltage divider to bring the 5V VESC/FOCBOX TX (transmit) pin down to 3.3V Bluetooth module RX (receive) pin. And you basically said that you have module marked as being 3.3V TTL. I think you do need resistors. It will (probably) work as is but it might also burnout (sooner or later).

Also, both diagrams are wrong. First one is using voltage divider for TX->RX and yet it connects to 5V VCC which makes no sense. There is nothing basically incorrect with second diagram but it is wrong for your usage (with voltage divider resistors). If you are going to use resistors, you do not connect last 5V pin but second to last 3.3V one. Keep in mind that image is showing VESC and not FOCBOX that has this plug rotated 180 degrees. Pinout is the same but rotated.
```

---
## \#6 Posted by: DavidBanner Posted at: 2017-08-17T01:21:18.849Z Reads: 224

```
I went with what @JohnnyMeduse said and connected without the resistor(s).

It's been working flawlessly since I connected it.
```

---
## \#7 Posted by: SilentException Posted at: 2017-08-17T01:31:47.342Z Reads: 219

```
As I said, it will probably work but for how long.

TLDR, if I had Bluetooth module rated for 3.3V, I would use 3.3V to power and send data to it and not 5V. Makes sense, no? :slight_smile:
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2017-08-17T01:38:15.327Z Reads: 215

```
If you prefer there is a 3,3v pin on the vesc
```

---
## \#9 Posted by: SilentException Posted at: 2017-08-17T01:39:22.228Z Reads: 211

```
I know, see post above.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-08-17T01:42:11.530Z Reads: 213

```
Sorry my bad ... 😅
```

---
## \#11 Posted by: ricoghardforth Posted at: 2018-03-21T15:22:01.818Z Reads: 139

```
I've just got 10 pairs of JST 2.0mm 7-Pin PH Housing Female Connector with Wire and Male Connectors if anybody in the uk needs one and willing to cover postage.

https://www.ebay.co.uk/itm/10-Sets-JST-2-0mm-7-Pin-PH-Housing-Female-Connector-with-Wire-and-Male-Connector/322615498309?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649

I'm just about to solder my HM-10 cable up.  
There still doesn't appear to be a consensus on to use the resistors or not. 
My HM-10 looks to be a cheap Chinese knock off without the crystal.  Does this make a difference.  
I'm also using the Hobby King Turnigy SK8-ESC.    
Also my VESC enclosure is aluminium will I have to make a slot and expose the PCB antenna to get reception. 
Thanks.
```

---
## \#12 Posted by: DavidBanner Posted at: 2018-03-21T15:25:52.853Z Reads: 128

```
been using mine for about a year without the resistor and no issues
```

---
## \#13 Posted by: Marksmoura Posted at: 2019-04-26T06:49:49.055Z Reads: 41

```
I have Firmware 3.52 and I connected a hc-05 I can connect to Bluetooth on the app but no values are showing.

I also added the resistors on Bluetooth rx

Update:
I can connect using Windows laptop to Bluetooth com and configure using vesc tool. Works well and also shows real-time data. 

Just the app cannot read values..
```

---
## \#14 Posted by: L3chef Posted at: 2019-04-26T08:11:39.883Z Reads: 33

```
Did you approve read/write or what it's called in english. App permission might be a better word
```

---
## \#15 Posted by: Marksmoura Posted at: 2019-04-26T08:23:59.875Z Reads: 29

```
I just have storage permission option.
If I check permission details I see also permissions about Bluetooth but this ones there is no option to enable or disable. 

I am running android 9 p20 pro
```

---
