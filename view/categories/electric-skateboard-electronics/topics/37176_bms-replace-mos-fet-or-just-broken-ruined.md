# BMS; replace MOS FET or just broken/ruined?

### Replies: 9 Views: 1287

## \#1 Posted by: GunnarK Posted at: 2017-11-02T14:10:19.515Z Reads: 100

```
Hi guys,

Having a 'little' problem here
I was recently working on my battery because the negative lead had come loose of the BMS.

Now I managed to create some sparks from shorting by letting the negative battery lead touch one of the MOS FETs on the BMS. (see picture) the middle lug of the MOS FET has the most 'damage'.

This caused some colouring on the solder, but worse is probably that it seems to be the cause of my BMS not fully charge the battery anymore (stops around 68% or 37volts)...
<img src="/uploads/db1493/original/3X/a/4/a4e8aaf1ef6df596e34497b3328e1ff088ad839a.jpg" width="666" height="500">.
Other than not charging fully the BMS is fully operational. Regenerative breaking also seems to work

Could this easily be fixed? Like replacing that MOS FET. Or could it be the case that more hardware is affected?
I don't have a voltmeter yet to test things, but maybe you can give some direction in the matter!

Thanks
```

---
## \#2 Posted by: SilentException Posted at: 2017-11-02T14:28:34.567Z Reads: 93

```
If thats the only thing destroyed it should be easy fix, it's not even SMD component. 

Removeink, look at the part name, order replacement, desolder/solder.
```

---
## \#3 Posted by: GunnarK Posted at: 2017-11-02T15:06:25.295Z Reads: 85

```
Alright I will look into that. Any idea how I can test if it is still functional?

It seems though (don't have my board disassembled) from the picture below that the 2 pieces of PCB are soldered together to allow for transfer between the two. Probably not the easiest to reassemble that nice and tightly..
<img src="/uploads/db1493/original/3X/4/1/41b5f80bca8fa0b64cecc2ad846ef31b13e011f2.png" width="450" height="338">

I have contacted Bestech for some advice and will report back here

EDIT: this video can probably help testing the mosfet. Wouldn't hurt to test it while it is still installed on the BMS, would it?
https://www.youtube.com/watch?v=gloikp9t2dA
```

---
## \#4 Posted by: SilentException Posted at: 2017-11-02T16:04:18.987Z Reads: 71

```
Ah, that's that "sandwich" BMS. Well, the boards can still be separated quite easily though, just 4 screws and a row of pins it seems. I would put a big blob of solder over all the pins and heat it up so it separates all at once. Then use a solder wick to pick up the solder and free the holes. But, If you're not sure about your skills regarding this then do not do it and /or give it to someone to do the replacement for you. Testing while installed is not recommended, you won't get reliable info.
```

---
## \#5 Posted by: GunnarK Posted at: 2017-11-02T16:59:47.073Z Reads: 62

```
Haha never heard of that term.
I don't have any way to suck the solder of the pins. But could try it with some leftover braided copper wire.

Probably best to let someone else do it though. I am not that confident with the soldering iron that I want to mess with such small parts

[quote="SilentException, post:4, topic:37176"]
Testing while installed is not recommended, you won't get reliable info.
[/quote]

Unreliable but could it be sufficient to see if it still works? Would be nice to see before I disassemble the BMS and take it apart.
That way I should be able to easily compare it with the other MOSFETS regarding amperage, I assume.
```

---
## \#6 Posted by: SilentException Posted at: 2017-11-02T17:33:31.786Z Reads: 54

```
I don't know what is the MOSFET part number or type but for starters, try measuring impedance between source and drain pins.
```

---
## \#7 Posted by: GunnarK Posted at: 2017-11-02T21:58:22.760Z Reads: 46

```
I can't find the part number anywhere on the internet. But hopefully 'Donna' from Bestech can answer that question shortly (;
[quote="SilentException, post:6, topic:37176"]
try measuring impedance between source and drain pins
[/quote]

Will do sir!
```

---
## \#8 Posted by: GunnarK Posted at: 2017-11-03T14:44:24.295Z Reads: 40

```
According to Bestech's Donna the MOSFET part number is:
AOS/AO8822/TSSOP-8

Quote: "The MOS part number is: AOS/AO8822/TSSOP-8."

Which leads me to this product:
https://guide.alibaba.com/shop/ao8822-aos-tssop-8-ic-free-shipping_56403798.html

I think Donna referred me to the wrong part :disappointed_relieved:
```

---
## \#9 Posted by: GunnarK Posted at: 2017-11-06T08:50:00.924Z Reads: 27

```
So I just received an answer from Donna regarding the wrong part:

> I asked my engineer, that MOS you found it can't use, he said the correct MOS item number should be: IRF3307 / TO-220AB

This seems to be the correct one!
http://www.irf.com/product-info/datasheets/data/irfs3307.pdf
```

---
