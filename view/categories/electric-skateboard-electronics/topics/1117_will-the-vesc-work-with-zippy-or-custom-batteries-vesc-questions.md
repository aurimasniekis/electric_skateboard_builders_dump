# Will the VESC work with Zippy or custom batteries? VESC questions

### Replies: 9 Views: 1632

## \#1 Posted by: barajabali Posted at: 2016-01-27T16:39:46.852Z Reads: 148

```
Every post i see about vesc it seems to be limited to space cells. my mind tells me that it'll work with any battery but I don't want to purchase 2 VESC's and it not work with my custom packs. 

Does the VESC Accept sensor wires?  I get that it doesnt really need them but my motors have em so might aswell use them.

Also, best place to buy VESC? 

Please excuse my ignorance.

thanks in advance.
```

---
## \#2 Posted by: laurnts Posted at: 2016-01-27T16:51:39.913Z Reads: 148

```
@barajabali Benjamin Vedder doesn't make VESC only to work with SPACE Cell, so you could use Li ion / Lifepo4 / lipo packs / what ever batteries as long as it could supply the power your motor needs.

You will have to check VESC site by Benjamin to check the voltage limit as I didn't remember them by heart.

VESC has a port for hall sensor, but again most of builders here use VESC because of it's low speed non cogging ability. I didn't mean to recommend you to buy small / cheaper ESC, but this is one of the best feature of VESC. I believe you could combine sensored and sensorless mode with the BLDC tool provided. I would recommend to just connect them and test what works best for you.

2 Best place you could get VESC:
@onloop - Enertionboard
@chaka - Ollinboard
At least those are the suppliers I would recommend :smiley:
```

---
## \#3 Posted by: barajabali Posted at: 2016-01-27T17:00:51.958Z Reads: 147

```
Thanks alot again man! i just burned out 2 of my old esc's and i need a replacement i thought id just take the time and upgrade. i think @chaka is in the US? okay so i guess im going with 2 VESC's. Anything else ill need other then the esc's themselves? what is a bldc tool? so i need a connector between the two esc's? 
http://www.ollinboardcompany.com/product/vedder-s-speed-controller
on his site he has a bunch of options for them.  I have my own bullet and power connectors so I should just get the basic one huh?

Sorry i know im asking a lot of questions! Im not new to the hobby at all, ive been doing this for a while! just the VESC.
```

---
## \#4 Posted by: longhairedboy Posted at: 2016-01-27T17:13:29.744Z Reads: 132

```
@barajabali  You might  want to double check but I feel like VESC will do 14S max, so whatever you're doing on your board should be fine. 

There are two ways to run dual VESCs. 1) you can split the receiver signal using a Y connector or 2) you can bridge the two VESCs to behave like one by using a jumper to connect the two CAN busses so that they can talk to each other. I prefer the latter method because i belevie it to be cleaner and makes better use of the VESCs capabilities in my opinion. 

VESC should work just fine on any battery chemistry. 

BLDC tool is the software you use to configure VESC over the USB port. There's a windows version available in addition to the original linux code that has to be compiled. ITs pretty easy to use. ITs required to get VESC up and running.
```

---
## \#5 Posted by: laurnts Posted at: 2016-01-27T17:16:26.654Z Reads: 117

```
Ollinboard is in US yes. You will need to connect both VESC with the CAN bus connector, Ollinboard sells them as well.
However you will still need to connect both esc power to the batteries. BLDC tool is the software you will need to use to upgrade firmware and set your VESC. Like it or not you will need to use them once you're into VESC. It's not that difficult, but would take some time to understand and configure.

If you already have your own connector, then you don't need the additional (only if you want to).

---

I am very new as well, start building my board on November last year without 0 knowledge of hobby parts and longboarding. I can't even longboard until a month ago :smiley:
```

---
## \#6 Posted by: barajabali Posted at: 2016-01-27T17:22:09.571Z Reads: 107

```
Thanks for the help!  

Okay so if they are connected using the CAN Bus connector, do I have to program each one separately or just one and it the other will mirror it? and right now im only running 6s. I have plans to upgrade soon though. @longhairedboy
```

---
## \#7 Posted by: barajabali Posted at: 2016-01-27T17:23:57.940Z Reads: 104

```
thanks alot!  okay so when i order ill just order 2 $110 single VESC. and a can bus connector. got it! now how does the VESC connect to my computer? micro usb?
```

---
## \#8 Posted by: laurnts Posted at: 2016-01-27T17:26:47.491Z Reads: 99

```
Yes but I suggest you ask @chaka if they already have the dual VESC config build. The difference is that they are connected together and one of the VESC has an upright USB port

http://www.electric-skateboard.builders/t/ollinboardcos-compact-dual-vesc/649

Yes you will need to buy a USB cable for that, it's the micro usb.
```

---
## \#9 Posted by: barajabali Posted at: 2016-01-27T17:28:27.479Z Reads: 91

```
okay great ill just wait for his input on this and place my order :)
```

---
