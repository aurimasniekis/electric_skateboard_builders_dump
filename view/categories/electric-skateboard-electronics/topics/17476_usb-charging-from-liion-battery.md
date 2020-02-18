# USB charging from Liion battery?

### Replies: 17 Views: 1694

## \#1 Posted by: motiuridentity Posted at: 2017-02-10T00:45:17.912Z Reads: 190

```
I am building an e-board with a 10S5P Li-ion battery (15000mAh). 
- 50A BMS
- 190kv 6355 motor from DIY, single drive
- VESC

**I was wondering how I could add a USB port for charging my phone.** I was told I would need a converter (buck converter?) to bring the voltage down from 36V to 5V but I am unsure where to go from here.
```

---
## \#2 Posted by: Tonto2k Posted at: 2017-02-10T01:26:35.647Z Reads: 183

```
The vesc has 5V 1 amp available by making a parallel harness from the receiver wires. You can use this if you want :)
```

---
## \#3 Posted by: motiuridentity Posted at: 2017-02-10T02:59:20.990Z Reads: 178

```
Well it's only 1A... not terrible but I'd prefer 2A. Either way, is there a guide on how to do it? I want to know out of curiosity.
```

---
## \#4 Posted by: smurf Posted at: 2017-02-10T03:06:10.802Z Reads: 174

```
The easy way would be to get a 36v to 12v step down converter and then get some USB port that runs on 12v

https://www.amazon.com/Motorcycle-Cigarette-Lighter-Splitter-Charger/dp/B00PBKO2YY/ref=sr_1_9?ie=UTF8&qid=1486696003&sr=8-9&keywords=12+volt+usb+adapter
```

---
## \#5 Posted by: Tonto2k Posted at: 2017-02-10T03:09:01.471Z Reads: 167

```
You just need to splice the power from the 3 wire receiver.

<img src="/uploads/db1493/original/3X/1/5/15312df713fff55d7381a6bb25d14772d24b1027.jpg" width="638" height="424">

I make my own, negative to negative, positive to positive (signal wire not connected for your USB)

The positive wire goes to positive usb, negative wire to negative usb.

Hope this helps.
```

---
## \#6 Posted by: willpark16 Posted at: 2017-02-10T03:54:08.083Z Reads: 156

```
I have one if u want it
```

---
## \#7 Posted by: smurf Posted at: 2017-02-10T04:03:18.123Z Reads: 160

```
This might work

https://www.amazon.com/DROK-Converter-Step-down-Transformer-Stabilizer/dp/B015CD5HLG/ref=sr_1_22?s=electronics&ie=UTF8&qid=1486699199&sr=1-22&refinements=p_n_feature_keywords_two_browse-bin%3A6004420011
```

---
## \#8 Posted by: motiuridentity Posted at: 2017-02-10T04:17:51.822Z Reads: 155

```
What exactly do you have? 

So far I am seeing some good options posted here. Thanks guys I will take a look.
```

---
## \#9 Posted by: jmasta Posted at: 2017-02-10T04:36:53.462Z Reads: 157

```
This is how I built my USB phone charger:  I have a BEC (13-60V) that regulates the full pack voltage to power my 12V rail.  Then I have a cheap $3 BEC (6-23V) that steps it down to 5V.  Basically I already had the 12V BEC, so for $3 more, why not?  Then I just soldered on positive/negative wires to the outer leads of a USB receptacle. Lookup the pinout on the google machine

But if just want a phone charger and nothing more, the easiest and cheapest method would be to use the 5V output from the VESC. However this requires the VESC to be on to do so
```

---
## \#10 Posted by: SeanHacker Posted at: 2017-02-10T04:37:33.458Z Reads: 152

```
Would something like this work?
https://www.amazon.com/gp/aw/d/B01MSK7ZAV/ref=mp_s_a_1_1?ie=UTF8&qid=1486699689&sr=8-1&pi=AC_SX236_SY340_QL65&keywords=2+pin+usb+port&dpPl=1&dpID=51kYDXoSRcL&ref=plSrch
```

---
## \#11 Posted by: willpark16 Posted at: 2017-02-10T04:48:38.790Z Reads: 142

```
A USB port with bec the same one torquevoards uses in his packs
```

---
## \#12 Posted by: Jcullinan09 Posted at: 2017-10-25T03:11:18.367Z Reads: 86

```
@Tonto2k I don't quite understand how you made a female type A USB port to charge a phone off of the VESC. Could you (or anyone reading this) explain how a USB port can be modified to come out of the VESC? Maybe a diagram would help... 
Thanks!!
```

---
## \#13 Posted by: Tonto2k Posted at: 2017-10-25T04:38:54.437Z Reads: 80

```
You use the "Batt" 3 pin connector on your R/C Receiver. The vesc supplies power to the receiver through whichever servo channel you have it connected to.

Therefore, the power for the usb is connected to the mal and female of the "Batt" pins. There should be three of them, usually they are labelled positive and negative.

You will need to wire in the positive wire from a female usb to the positive of the "Batt" pins and a the negative from the usb to the negative of the "Batt".

Thats how I do it anyway :slight_smile:
```

---
## \#14 Posted by: Jcullinan09 Posted at: 2017-10-25T04:44:10.160Z Reads: 76

```
I think I get what you are saying, but would you happen to have any pictures? Or links to the Female USB port you used?
```

---
## \#15 Posted by: Tonto2k Posted at: 2017-10-25T05:02:29.240Z Reads: 76

```
I don't have any pictures mate as my board is in bits at the moment.

Basically you take this cable and cut off the male bit:

http://www.ebay.com.au/itm/30cm-Panel-Mount-Extension-Cable-USB-2-0-Male-to-Female-Extension-Port-AdapterAT/391886727452?hash=item5b3e44e91c:g:1FgAAOSwAKxWV8nF

Wire the positive and negative wires from the female usb into a jst connector such as this:

https://www.ebay.com.au/itm/New-200mm-helicopter-lipo-Battery-plug-JST-connector-Male-for-Lipo-connection-WS/263109589300?hash=item3d428db934:g:XG4AAOSw9NdXqwH0

Then plug the jst connector into the receiver "Batt" positive and negative pins.

Job done !
```

---
## \#16 Posted by: Tonto2k Posted at: 2017-10-25T05:03:17.953Z Reads: 70

```
You can also use jst connectors off a pc case if you have any lying about :)
```

---
## \#17 Posted by: Jcullinan09 Posted at: 2018-10-04T22:41:34.105Z Reads: 35

```
Where can an individual like myself find a female USB A to servo cable like the one @Tonto2k has?? 
THANKS!
![image|638x424](upload://jF2CrABbrHsxKSskiU1Ey14EWDl.jpeg)
```

---
