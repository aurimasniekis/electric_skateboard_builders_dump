# Best place to get 5Volts from ?, &hellip;using Vesc and GT2-B reciever

### Replies: 17 Views: 2841

## \#1 Posted by: Randyc1 Posted at: 2016-02-25T00:07:41.776Z Reads: 314

```
I will be using a "Drok" Voltmeter on my eboard , it can be powered direcly from the battery from to 3-30V,..
but i will have 10S battery pack so 42 Volts .

Where is best place to Tap into to get 5V to power my Voltmeter?..., i'm using the Vesc and the GT2-B Reciever.


Thanks.
```

---
## \#2 Posted by: evoheyax Posted at: 2016-02-25T00:48:41.206Z Reads: 309

```
Idk actually but am curious if someone else who knows more could elaborate. I use the recover to power 2 fans and my lights.
```

---
## \#3 Posted by: delta_19 Posted at: 2016-02-25T00:54:51.554Z Reads: 307

```
isnt the point of the voltmeter to show you what your batteries are pumping out? connecting them to anything other then the battery leads would give you a read out of that source so in your case a constant 5V, you would no longer know how much juice you have.
```

---
## \#4 Posted by: Sharkface Posted at: 2016-02-25T01:00:57.135Z Reads: 303

```
http://www.amazon.com/gp/product/B0194SKADU?psc=1&redirect=true&ref_=oh_aui_detailpage_o02_s00

I just got these guys but I have yet to test them. There are some sbecs on hobbyking that will suport that 12s lipo.... but there are multiple reviews on the page stating that they will die. So I went with these dudes, especially since they offer a 12v version as well

Good luck my man!!!!!
```

---
## \#5 Posted by: onloop Posted at: 2016-02-25T05:12:59.060Z Reads: 283

```
I am confused... what voltage do you want to read?

Does your volt meter need 5v auxiliary power to work?
```

---
## \#6 Posted by: paragon Posted at: 2016-02-25T05:26:13.847Z Reads: 279

```
Warning, you may blow your receiver trying to pull 5v from it; they aren't particularly rugged. I'd go for a BEC
```

---
## \#7 Posted by: trbt555 Posted at: 2016-02-25T06:12:30.724Z Reads: 270

```
For the confused: that type of voltmeter needs a separate power supply, not just the voltage you're measuring. You can't just tie both together because the measuring range is higher than the max allowable supply voltage.

For @Randyc1: 
There's a 5V supply on the VESC, it's on pins 1 and 3 of header P3 : [schematic][1]
It can supply up to 1A but be very careful not to short it or you'll blow the DRV8302.

  [1]: https://raw.githubusercontent.com/vedderb/bldc-hardware/master/design/PNGs/Schematic-1.png
```

---
## \#8 Posted by: RogerD Posted at: 2016-02-25T19:19:18.015Z Reads: 247

```
If you are not confident with attaching to P3 just take your power from the same pins your receiver is using.  You can use a servo Y lead. It's rated at the same 1A - its the same power source I believe. Your volt meter will use a few milliamps to power itself.
```

---
## \#9 Posted by: Randyc1 Posted at: 2016-02-25T23:55:16.041Z Reads: 234

```
Yes , needs 3-30 volts to power Voltmeter  ,..Has 3 wires ,Black (ground), Red ( power supply) ,White (measuring Battery Pack)
```

---
## \#10 Posted by: Randyc1 Posted at: 2016-02-26T00:26:36.806Z Reads: 230

```
Thanks Roger , Trbt555.

Yes Maybe taking from reciever is less risky!

So i can just tap onto the Pos & Neg of reciever wires correct ?
```

---
## \#11 Posted by: RogerD Posted at: 2016-02-26T09:31:34.769Z Reads: 211

```
Yep - there are three pins for the receiver connection + - and signal. Red, Black, White(or orange). You want the red and black. You are not technically tapping into the receiver - you are tapping into the VESC 5v power rail :smile:

Your volt meter, as you have discovered, will have three wires - red and black for battery / ESC main power connections and another low voltage white wire for powering the LED display - this is the one you want going to the VESC receiver + pin. No need to run the earth here. YOu are getting that from the main battery black and red wires.
```

---
## \#12 Posted by: Randyc1 Posted at: 2016-02-26T15:05:13.559Z Reads: 203

```
Hmmm Roger, now im confused ?

  (WHITE Voltmeter wire) is the one that measures my 10s4p battery.

Black will tap to black on Reciever .(ground)
Red will tap to red on Reciever . (5v Power for voltmeter)


This Voltmeter is wired just like Trbt555 explained earlier.
```

---
## \#13 Posted by: RogerD Posted at: 2016-02-26T16:18:18.463Z Reads: 191

```
my apologies. Was in a rush. You are correct.

White goes to the main battery supply.
Black to any earth - either the main battery, or the earth on the receiver input pins on the VESC.
Red (to power the meter) goes to the live 5v pin in the receiver inputs on the VESC
```

---
## \#14 Posted by: Bender Posted at: 2016-05-20T13:22:44.575Z Reads: 176

```
Were you successful in getting your volt meter hooked up?
I'm thinking of using the same type
```

---
## \#15 Posted by: Randyc1 Posted at: 2016-05-20T20:33:29.817Z Reads: 163

```
Yes !, i got 5v to power the Voltmeter from tapping into the reciever's (+ & -)  ,...then 3rd wire (white) on the Pos side of my battery pack to read voltage of pack ,...works perfectly.

My voltmeter is the "Drok" , 3 wire version .
```

---
## \#16 Posted by: Pablo_702 Posted at: 2016-07-27T19:40:17.740Z Reads: 130

```
Can u take a picture of the wiring next time you open your enclosure pls
```

---
## \#17 Posted by: GhettoFab.rictation Posted at: 2017-11-09T08:58:39.626Z Reads: 46

```
Can we use step up converter to power lights from these pins is that possible? As well as fan for vesc?
```

---
