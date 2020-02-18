# Lowering output DC voltage from 5.2v to 4.2V to charge a 18650 battery pack

### Replies: 8 Views: 1289

## \#1 Posted by: Eboosted Posted at: 2017-04-08T02:24:02.464Z Reads: 75

```
I need to manually balance one of my low voltage packs.

I have a 5.2V 1.35 cell phone charger, what would be needed to lower the output voltage to 4.2V?
```

---
## \#2 Posted by: Eboosted Posted at: 2017-04-08T02:38:10.174Z Reads: 72

```
I found another power supply, it has 4.35V output, would it be safe to use that one?

I'll keep an eye on the pack voltage all of the time.
```

---
## \#3 Posted by: PXSS Posted at: 2017-04-08T02:42:51.636Z Reads: 66

```
Is this on the pack that you've discharged to 0 several times. Remember what I said about more likely to catch on fire?
```

---
## \#4 Posted by: TranxFu Posted at: 2017-04-08T10:16:09.814Z Reads: 52

```
Either use resistors or get a step down converter. Pay attention that to the voltage range it can adjust to.

EDIT:: but don't fiddle with sketchy packs.
```

---
## \#5 Posted by: Eboosted Posted at: 2017-04-08T16:14:44.658Z Reads: 40

```
That packs a has already been discarted, after I saw it had zero volts. I replaced it with a new pack of brand new Samsung 25R 18650, but I made a mistake and didn't balance the pack before building it, that pack reached 1.75V once but recovered. I'd like to balance it without disassembling.

Hope to get some suggestions on how to do it.
```

---
## \#6 Posted by: jmasta Posted at: 2017-04-08T16:38:11.202Z Reads: 33

```
Reposting.... 

But if you want to simplify it even further... The leads on the power resistor linked below would fit in the JST balance plug. Just attach a voltage meter to each end of the resistor to monitor the cell during discharge. The switch is not essential; it just makes it easier to compare voltage under 2A load to resting voltage

So all you need is a 10W+ power resistor and a DVM. Done.

[quote="jmasta, post:126, topic:19302, full:true"]
You could just make a simple discharge device to manually bring down the voltage of each cell.  Basically you'd just attach a resistive load to the (+) and (-) terminals of one cell.

For a voltage range of 4.2V to 3.7V, a **2 Ohm resistor** would give you about **2A discharge**

The maximum power dissipated would be about **8.8W**.  Therefore you'd need to buy high wattage resistor, sometimes called a power resistor.  10W would do. 20W resistor would be better.  

Something like this 20W resistor would work:  
https://www.amazon.com/20W-Cement-Resistor-TOOGOO-Resistors/dp/B01GKWDTW2/ref=sr_1_2?ie=UTF8&qid=1491507211&sr=8-2&keywords=2+ohm+20w+resistor


Or on Amazon Prime for USA guys:  https://www.amazon.com/uxcell-Wire-Wound-Cement-Resistors/dp/B0087ZDDOU




<img src="/uploads/db1493/original/3X/0/f/0f9465748bb7029686671bb92edd39f23e6b2d29.jpg" width="332" height="500">

The pins could just be breadboard jumpers. You would unplug your balance plug from the BMS, and then stick your two discharger terminals into two adjacent pins on the JST plug (corresponding to the cell you're trying to discharge).  Check the cell voltage with the DVM.  Then activate the switch to apply a ~2A load to the 20W (2 Ohm) resistor.  Continue draining the cell until it matches the voltage of your lowest cell (cell 5 for you @Eboosted). Turn off the switch to see resting voltage. Keep toggling back and forth until the resting voltages match.

Then do this for every cell, bringing down the voltage of each cell individually until they match your lagging cell.  If done correctly, you've just manually balanced your pack without disassembling it. Your BMS should now be able to balance them since they are all roughly the same voltage

Note:  Would be a good idea to include a **fuse** as well!!
[/quote]
```

---
## \#7 Posted by: Eboosted Posted at: 2017-04-08T18:17:05.987Z Reads: 24

```
@jmasta This was indeed really helpful, thanks a lot for the time to write this down.

I'll do it today, I'm on my way to the electronic shop
```

---
## \#8 Posted by: surprisebirthday Posted at: 2017-11-19T18:53:50.298Z Reads: 17

```
This is awesome.  My cells are out of balance as well, and this looks like the best solution I've read so far.

For jmasta or anyone who might know, is it necessary to connect the power resistor to the JST balance plug?  Could I instead just connect the leads on the power resistor to a pack that I want to lower the voltage on?  For example, connect the leads to the sides of the pack that I highlighted below:

<img src="/uploads/db1493/original/3X/f/e/fedbcb3a8d7ff449f3d1e5d06caf40ee1da61ce1.JPG" width="500" height="500">

I ask because my balance leads are all hot glued to the JST balance plug.  I could try to remove it, but I am afraid I'll accidentally damage my BMS.  Here's a picture of the JST balance plug, in case someone sees an easy way to deal with it.  If it helps, this is an Enertion Spacecell, 10s3p.

<img src="/uploads/db1493/original/3X/6/4/64524802f5a49b5bbbeae756e6d7112e9e5b4b6a.JPG" width="500" height="500">

Thanks, guys.  Looking forward to rehabilitating my gimpy battery.
```

---
