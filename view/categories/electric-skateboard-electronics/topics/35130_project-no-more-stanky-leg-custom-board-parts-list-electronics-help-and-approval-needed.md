# Project no-more-stanky-leg / Custom board / Parts list electronics / Help and approval needed

### Replies: 12 Views: 773

## \#1 Posted by: Guyer Posted at: 2017-10-08T21:44:47.467Z Reads: 116

```
Hey guys!
Totally new on the site, already lovin' the community! I wanna build my first electrical board, and after a lot of research on the different components needed i have come to this setup:

**Motor**	:                KEDA 63-64 190KV Brushless Outrunner 10S 2000W
https://hobbyking.com/en_us/kd-53-30-high-voltage-brushless-outrunner-190kv.html

**Battery**         :           ZIPPY Flightmax 5000mAh 3S1P 20C 
_(Thinking of 9S, so a series of 3 of these??)_
https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html

**Speed Controller**  :   Maytech Benjamin Vedder Electronic Speed controller VESC for electric longboard _
_(I have read that the VESC is A LOT better than a ESC, and is worth the money?)_
http://www.ebay.com/itm/Maytech-Benjamin-Vedder-Electronic-Speed-controller-VESC-for-electric-longboard-/302200711613?hash=item465c90e9bd:g:tRkAAOSwiDFYPFHa

**Transmitter**	:        2.4GHz Radio Remote Controller Receiver Transmitter Kit For Electric Skateboard 
_(Can i plug this reciver straight in to the VESC or do i need a cable?)_
http://www.ebay.com/itm/2-4GHz-Radio-Remote-Controller-Receiver-Transmitter-Kit-For-Electric-Skateboard-/282570883443?hash=item41ca898173:g:Ua8AAOSwRMtZY4CD

**Voltmeter**	   :            12V LCD Acid Lead Lithium Battery Capacity Indicator Voltmeter Voltage Tester
http://www.ebay.com.au/itm/272581713717?ssPageName=STRK:MESINDXX:IT&_trksid=p3984.m1436.l2649

**On/off button**  :        19mm Self Locking Blue LED 24V Stainless Steel Push Button Switch SPDT D5I7
http://www.ebay.com.au/itm/19mm-Self-Locking-Blue-LED-24V-Stainless-Steel-Push-Button-Switch-SPDT-D5I7-/292081451756?epid=526533271&hash=item44016942ec:g:g48AAOSwnF9Y6s-1

**Charger**       :           Any ideas? I would prefer a solution that can charge all batteries at once, through a exterior plug, so i dont have to disassemble the board to charge :) 

What do you guys think? Missing something? Should i swap some parts? Another batterypack? Would really appreciate if one of you esk8 veterans could go through it :) 
As i said, im pretty new to the subject but have read so much that i now only see the sollution to write a thread myself. I dont have an enormous budget and i live in Denmark where import taxes are pretty high for non-EU countries :slight_smile: 

Best regards
Jacob
```

---
## \#2 Posted by: Brycehoosiers Posted at: 2017-10-08T21:53:46.306Z Reads: 102

```
Wouldn’t recommend the maytech VESC because they cheap out on as many parts as possible so it’s more likely to break. I’d go for the torque boards VESC or Ollin boards VESC
```

---
## \#3 Posted by: bigben Posted at: 2017-10-08T21:55:06.871Z Reads: 99

```
For a switch you might be better off with an xt90-s loop key. That switch will burn out. 
Have a search and read about anti spark switches.
```

---
## \#4 Posted by: darkkevind Posted at: 2017-10-08T21:58:11.485Z Reads: 97

```
The push button won't work unless you have an anti spark (Vedder type) switch to use it with. Esk8 pulls from too many amps for most little switches like that that are rated for no more than 10A, probably only 6A.

If you want to charge the batteries without disassembling your board you'll need a 9s 60-80A BMS. Either that or run 3 XT60/90 connectors to the outside of your enclosure as well as each batteries' respective balance connectors...
```

---
## \#5 Posted by: Guyer Posted at: 2017-10-08T22:14:24.777Z Reads: 84

```
Thanks a lot guys! l'll go with the xt90s loop key i think :) @darkkevind can you link such a bms? i can only find one https://www.alibaba.com/product-detail/9S-80A-28-8V-BMS-PCM_60190504932.html but i would have to order 2...  Seems like 9s setup is not very common? could i use a 10s with my 9s setup?
```

---
## \#6 Posted by: bigben Posted at: 2017-10-08T22:19:46.785Z Reads: 79

```
Perhaps something from this company?
http://bestechpower.com/333v9spcmbmspcbforli-ionli-polymerbatterypack/PCM-D131.html
```

---
## \#7 Posted by: Guyer Posted at: 2017-10-08T22:27:05.436Z Reads: 80

```
thanks a lot!
I've contacted them for pricing/ordering and payment :) 
Do i need any additional cables or is itjust plug and play with the secure connecters and power wires from the batteries ? Im a little confused about the whole wiring diagram/setup :)
```

---
## \#8 Posted by: bigben Posted at: 2017-10-08T22:43:29.061Z Reads: 76

```
There will probably be an element of soldering involved. 
I'm not familiar with the 9s BMSs but the 10s ones have been popular with people building 10s lipos batteries from 5x2s batteries.
```

---
## \#9 Posted by: darkkevind Posted at: 2017-10-08T23:05:56.910Z Reads: 69

```
You could get a much less amp BMS of you're willing to bypass the BMS for discharge, and only use it to charge, which is what I do with my 8s4p li-ion pack I made...

Try 9s 10A or even less...

You can't use a 10s BMS for a 9s setup, they HAVE to match.
```

---
## \#11 Posted by: Guyer Posted at: 2017-10-09T00:02:01.657Z Reads: 65

```
I've looked around a bit @darkkevind @bigben :)  
Would these: https://hobbyking.com/en_us/zippy-flightmax-5000mah-5s1p-20c.html 
work as 2*5s for this bms: http://www.ebay.com/itm/10S-36V-35A-Li-ion-Battery-Protection-Board-BMS-PCB-Balance-fits-Ebike-Escooter-/202017567874?hash=item2f092f7482:g:3JwAAOSw4gNZiTGf 
with this power supply: http://www.ebay.com/itm/42V-2A-Lipo-Battery-Scooter-Balance-Charger-For-Electric-Self-Balancing-2000mA-/191942920872?hash=item2cb0b08aa8:g:mp4AAOSwZVlXqyPZ ?
```

---
## \#12 Posted by: darkkevind Posted at: 2017-10-09T06:36:11.840Z Reads: 50

```
The batteries are only rated for 20c so possibly a little under powered, try at least 25c, preferably 30-50.

The BMS looks fine if you're going to bypass the BMS for discharge. This means that you're not going to use the BMS' output wires to power your ESC and ultimately your motor, you'd use the output wires directly from your batteries and you'd only use the wires from the BMS to charge the batteries.

There are risks to this method, but if you're careful and check your cells regularly, you can set the battery cut off level in your VESC so that it won't discharge your batteries too much.

I suggest you do a bit more searching on this forum for more information about that.

The charger/PSU should be fine.
```

---
## \#13 Posted by: pat.speed Posted at: 2017-10-09T07:13:11.006Z Reads: 41

```
Hey man this is nearly identical to my build. Same motor, batteries, and I was going to use that Vesc but changed at the last minute to a 6s car esc. DO NOT GET THAT ESC unless you have the time to fix or replace it quite a few times (it could work well for you but most people that use maytech vescs have them blow up quite quickly). Btw I love that motor has heaps of power
```

---
