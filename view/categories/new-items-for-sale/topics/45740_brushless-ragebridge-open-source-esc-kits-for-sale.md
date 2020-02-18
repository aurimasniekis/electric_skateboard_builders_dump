# Brushless Ragebridge - open source ESC *kits for sale*

### Replies: 10 Views: 1102

## \#1 Posted by: goldenHusky Posted at: 2018-02-06T18:37:44.658Z Reads: 236

```
Read more about this open source ESC here 
http://e0designs.com/products/brushless-rage/


I have a total of 5 kits of the "Brushless Ragebridge" 6-FET ESC  for sale.


[img]http://up.picr.de/31748430zf.jpg[/img]

[img]http://up.picr.de/31748431sy.jpg[/img]

[img]http://up.picr.de/31748432jl.jpg[/img]

One kit contains:

* components according to the official BOM
* two program adapters + cable (in case one of them doesn't work)
* aluminium heatsink
* pcb of the powerboard and the signalboard

Notes:

* power mosfets from the BOM were replaced with FDBL86363-F085 due to lack of availability
* the drill holes on the heat sink are off, you may have to drill two new holes for a proper fit
* the pin header are not included (were left free at the BOM paper)
* Some parts are/were really hard to find/get, I had to order parts from 4 different traders and resellers worldwide
* I will print a list and tape every component right next to the text, I do this with utmost care and check it multiple times, but if sh*t happens please get the component on your own as I don't want to ship a 50 cent part

Price per kit is 80€.
This is what it cost me, so there is no room for negotiation.

Furthermore I have one stencil for the powerboard and one for the signalboard pcb, each is 20€.
I do also have some bare power and signalboards left, selling both for 15€.

Shipping costs below:

Within EU:
5,50€ economy (5-15 days) no tracking
6,90€ priority (2-4 days) no tracking
9,75€ priority with tracking

Rest of the world:
10,15€ economy (10-20 days) no tracking
12,25€ priority (4-8 days) no tracking
15,10€ priority with tracking

Since the shipping cost is quite high, I want to clearify that I don't squeeze myself extra money out of that.
Feel free to check the shipping rates here at the calculator of the Austrian post service (envelope format will be C4/B4) https://www.post.at/tarifrechner.php?land=SZ&gewicht=100&gewicht_art=g

Thanks!

Fabio
```

---
## \#2 Posted by: SilentException Posted at: 2018-02-06T19:07:17.187Z Reads: 212

```
Very interesting! Did you had time to build one and do a board test?
```

---
## \#3 Posted by: goldenHusky Posted at: 2018-02-06T19:20:14.835Z Reads: 215

```
@SilentException
I didn't and I won't have time in the next few weeks, so I sell everything.
```

---
## \#4 Posted by: SOICDIP Posted at: 2018-02-06T20:48:07.419Z Reads: 204

```
[quote="goldenHusky, post:1, topic:45740"]
I will print a list and tape every component right next to the text, I do this with utmost care and check it multiple times, but if sh*t happens please get the component on your own as I don’t want to ship a 50 cent part
[/quote]

That's completely understandable, but it might be nice to stick a couple of extra spares especially for the smaller SMDs because if you lose any of them, you have a non functioning ESC.
```

---
## \#5 Posted by: goldenHusky Posted at: 2018-02-06T21:06:14.357Z Reads: 181

```
I'll be happy to do that :wink:
```

---
## \#6 Posted by: Vanarian Posted at: 2018-02-07T17:07:29.541Z Reads: 152

```
Looks cool, maybe a nice competitor for the VESC ? 

I don't know well the SimonK controllers, have seen some used for less powerful applications but here that's not the case with 60A and 120A respective continuous ?
```

---
## \#7 Posted by: goldenHusky Posted at: 2018-02-07T23:57:40.247Z Reads: 134

```
Yea, I've seen some video footage of an electric gokart powered by this ESC so.. it would be very interesting how it performs in comparison to the vesc since it is also programmable etc.
```

---
## \#8 Posted by: marcoccio Posted at: 2018-02-21T04:34:42.744Z Reads: 120

```
Can you make a kit for the 12 mosfets version?
```

---
## \#9 Posted by: goldenHusky Posted at: 2018-02-21T09:58:02.636Z Reads: 107

```
Unfortunately not @marcoccio
```

---
## \#10 Posted by: goldenHusky Posted at: 2018-03-25T17:36:42.130Z Reads: 86

```
**UPDATE**
I've had nothing to do this afternoon so I soldered some controllers


[url=https://ibb.co/nuHAUn][img]https://preview.ibb.co/iRxAUn/IMG_5439.jpg[/img][/url]

[url=https://ibb.co/matH9n][img]https://preview.ibb.co/n7UqUn/IMG_5441.jpg[/img][/url]

[url=https://ibb.co/hnjw27][img]https://preview.ibb.co/fUZJFS/IMG_5442.jpg[/img][/url]

However I'm stuck on flashing the firmware via the KKMulticopter Flashtool and the Afro USB Programmer, the procedure is the same as when flashing code on any Atmega8 chip. I get timeout and Java compatibility errors.. spent hours for nothing.

So if someone has more experience softwareside or with flashing chips with an usb programmer in general and would like to perform this last step.. they are still 80€ each, though they are pre-soldered now. They retail for 150$ from the manufacturer.

EDIT: I believe I know why it doesn't work, I need another programmer who can write fusebits, the Afro Programmer can't set up blank chips, just ordered a couple.
```

---
