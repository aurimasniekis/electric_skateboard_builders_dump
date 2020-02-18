# Trampa Street/Urban Carver Battery Question

### Replies: 11 Views: 909

## \#1 Posted by: NoWindCH Posted at: 2018-03-12T21:14:32.251Z Reads: 158

```
Hallo everyone

I am from Swizerland and i build my first elektric Skatebord.
My deck i have is a Trama street and urban carver.
At the moment i driv it with the Trampa motors with 118kv and two Alien Power 6S 10ah 35C and two VESC 6.14.

Now i want to built a baterie pack in the underbord batterybox.

Firs i chose the Samsung INR21700-48G - 10A (35A) i have now 50 pice of them here.
https://www.akkuteile.de/samsung-inr21700-48g-4800mah-10a-35a-3-6-3-7v/a-100625/

In the past now i think my batherypak with 12s 4P are too small with 40A for two motors.

May i put on the APS Motors hwo runs with (6374S 170KV 3200W) 800Watt mor than the Trampa ones but only on 10S, so they drive even on more amps am i right?

Shuld i buy these ones? iJoy 21700 - 3750mAh With 25S and 40A Peak.
https://www.akkuteile.de/ijoy-21700-3750mah-lithium-ionen-akku-3-6v-3-7v/a-100665/

So then i use the oder 50 pice in a big portabel speaker i build.

And my other question is wich BMS is the best for me?
How can i get an DieBie BMS? (May two i want to build an ofroad board too. with the bigest Motors i can fit on the Directdrive etoxx Mounts.)

LG Pascal
```

---
## \#2 Posted by: FredrikHems Posted at: 2018-03-12T21:19:54.024Z Reads: 141

```
I dont know about the quality of the iJoy, but I will suggest you to go with Samsung 30q (20A 3000mAh) or the Sony VTC6 («35»A(more like 20) 3150mAh). Both these are 18650 cells, in these are what about everyone here use :slight_smile:
```

---
## \#3 Posted by: Acido Posted at: 2018-03-12T21:24:36.952Z Reads: 134

```
iJoy seems fake, huge discharge and huge capacity...
I would go with the standard 30Q cells, much cheaper almost the same mah if you put one more in paralel
I would suggest a bestech bms or the diebie bms, bestech proved to be very good I think that the diebie one also did

For one 48G battery you can get 3x 30Q ones... much cheaper to go with 30Qs

Also where do you live, I visit Switzerland all the time
```

---
## \#4 Posted by: NoWindCH Posted at: 2018-03-12T22:21:31.004Z Reads: 126

```
Thank you for the fast reply

On the carver desk i have only 60cm space for the Bateries,BMS and two VESCs also the wiring... thats the thing

I will loock tomorow ho much space i have mor with 18650 Cells. May i can build an 12s 5p.

What do you guys think abaut this BMS?
https://www.energusps.com/shop/product/tiny-bms-s516-150a-750a-36?category=4
its not cheap but i want good parts xD

So this or one from the bestech only the DieBie i dont know how to get. I wrote him a massage but i got no answer.

Thats cool @Acido  i live in Aargau in Holziken. its near to aarau.
```

---
## \#5 Posted by: Acido Posted at: 2018-03-12T22:26:03.434Z Reads: 109

```
12s5p is a big battery  650wh
That bms seems really cool and compact
It claims huge numbers and has some great freatures, I would do some research on it

But also you can save some money and get the bestech one and a bluetooth module for about half the price

I just returned from luzern few days ago btw
```

---
## \#6 Posted by: NoWindCH Posted at: 2018-03-12T22:37:12.306Z Reads: 104

```
yes thats wuld be grat if it fits in thee box :smiley:

Yes because its so compact i loockt at it.  From Bestech it wuld be this one,m right?
http://bestechpower.com/444v12spcmbmspcbforli-ionli-polymerbatterypack/PCM-D131.html

Hmm.. so maby we can make a long range thest with the bord an travle back with ÖV. HAHA But 41km, its a realy long distance with one charche.
```

---
## \#7 Posted by: banjaxxed Posted at: 2018-03-13T11:03:47.677Z Reads: 86

```
The DieBieMS group buy is all done but since JTAG decided to open source the design you could use produce your own.

If not maybe look at what @SimosMCmuffin is doing with a new BMS twin board design, you're being spoilt now 👋

FlexiBMS
http://www.electric-skateboard.builders/t/flexibms-first-prototype-kicad-project-files-released-flexible-configuration-and-charging-bms/46117
```

---
## \#8 Posted by: NoWindCH Posted at: 2018-03-13T19:56:34.136Z Reads: 72

```
I do not think, that i can build an BMS by my self. without spending muney for broken parts and stuff for build... hahah

I can wery well weld every kind of steel, without a problem. I do it every day at work.
so i make the endings of the baterybox out of  aluminium and paint it red.

Can some one tell me how this work, when the VESC charch the batery with the Tiny BMS s516 - 150A/750A?

This BMS has seperad Load and Charche inputs.

So when i brake the batery will be charching without balancing? Or is there a problem for the BMS when there come electricity back in to it at the Loat ports.

There are meshuring abaut the iJoy 21700 should i trust them?
![iJoy 40A 3750mAh 21700 CC NEW BATCH TESTS|690x340](upload://hC0sf43EBhNvQBKv7vWVpbZdRUu.jpg)

just because its an unknown faktory, not like Samsung, Panasonic or LG...

Yes i know i give much more money, just for thaving the best i can in my board.
```

---
## \#9 Posted by: FredrikHems Posted at: 2018-03-13T22:04:15.308Z Reads: 63

```
wow, seems like the iJoy shit only have a capacity of 1900mah at 40a! 

I would definitely go for a trusted cell like 30q
```

---
## \#10 Posted by: NoWindCH Posted at: 2018-03-14T19:25:11.996Z Reads: 56

```
Yes, i will chose the Sony VTC6!

Can some one answer my question abaut the BMS, when i have difrent load and Charge Ports?
```

---
## \#11 Posted by: NoWindCH Posted at: 2018-03-15T18:11:50.607Z Reads: 46

```
Hey what do you guys think abaut this idea?

The baterys have 18mm in higt and i have 25mm space..
i cud chose a very narrow bms like this one:
http://bestechpower.com/communicationbms/BMSD328.html
and put it over the 18650 cells.
```

---
