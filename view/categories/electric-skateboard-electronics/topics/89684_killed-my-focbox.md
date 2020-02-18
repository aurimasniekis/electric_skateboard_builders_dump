# Killed my focbox?

### Replies: 20 Views: 309

## \#1 Posted by: JensSjogren Posted at: 2019-04-07T07:51:52.705Z Reads: 127

```
So yesterday i was doing some donuts on a gravel field and suddenly my board stopped working. in heinsight i'm not really surprised by that considering i was constantly pushing it in deep gravel for about 20 minutes.. 

Anyways, opened up the ESC case and the focboxes was really hot for sure, carried the board home and started to locate the problem, the slave Focbox seems to be fine and both motors spin when plugged into it, the master focbox however gives no power to the motor. it starts up just fine and the signal led lights up. When hooked up to Vesc-tool it gives no error messages, running motor detection gives me green values but it does not react with the motor, nothing happens. 

I opened up the case to see if there was any fried componants, not really sure what to look for here but i can't find anything that looks damaged, i'll post pictures for someone that knows something about circuit boards. Well i guess what i'm looking for is if anyone experienced the same problem and if there is a fix to it. since i can start the focbox and connect it to the computer it isn't completely dead right.


Setup
-2x turnigy sk8 6374 192kv motors
-12s9p 30Q pack with charge only bms and fused for discharge.
-2x focbox 
-gearing ratio 1:6 

settings per focbox
motor max A = 100
motor min A = 45

battery max A = 50
Battery min A = 12

![20190406_205756|375x500](upload://2CEeojSvmoVLUa8yI99jsscmhYT.jpeg) 
![20190406_205821|375x500](upload://6Wd7Mx9pAAPABe1LAGxArq0vSTA.jpeg)
```

---
## \#2 Posted by: b264 Posted at: 2019-04-07T07:57:14.631Z Reads: 120

```
Hand-test the motors -- and if they both pass, switch which motor is connected to that ESC and see if it switches which one works.
```

---
## \#3 Posted by: b264 Posted at: 2019-04-07T07:58:01.356Z Reads: 119

```
That bottom photo I see bad signs.  Please post a higher resolution photo of the direct FETs that isn't blurry.
```

---
## \#4 Posted by: JensSjogren Posted at: 2019-04-07T08:18:34.304Z Reads: 118

```
With hand test you mean? 

I tried both motors with both focboxes seperatly. 

The focbox that was running as slave in the dual setup is able to spin both motors. 

The "dead" one that was running as master isn't able to spin any of the motors

I'll take better photos when i get home :)
```

---
## \#5 Posted by: b264 Posted at: 2019-04-07T08:41:36.589Z Reads: 99

```
[quote="JensSjogren, post:4, topic:89684"]
With hand test you mean?
[/quote]

I think @dareno has it saved, or search for it
```

---
## \#6 Posted by: Gamer43 Posted at: 2019-04-07T08:46:51.658Z Reads: 100

```
The gate drive side of the DRV8302 is dead.

Same thing happened with one of my friend's TB ESCs. FOC detection gave green values, but a sanity check showed those values were nonsensical. 
Further probing revealed that the bootstrapped driver on phase A, and the GVDD charge pump were fried.

Most likely need to replace the DRV8302.
```

---
## \#7 Posted by: JensSjogren Posted at: 2019-04-07T09:20:59.941Z Reads: 91

```
Okay, shouldnt it give me a fault code in the vesc tool?
```

---
## \#8 Posted by: Gamer43 Posted at: 2019-04-07T09:22:24.339Z Reads: 91

```
Wasn't the case for my friend's ESC :man_shrugging:

What values do you get for resistance and inductance during FOC detection?
```

---
## \#9 Posted by: JensSjogren Posted at: 2019-04-07T09:24:10.461Z Reads: 86

```
Crazy high values, didnt memorize them but i noticed they were waaay higher than usuall
```

---
## \#10 Posted by: Gamer43 Posted at: 2019-04-07T09:27:06.382Z Reads: 83

```
Same thing happened with me. 

got like 28600mOhm resistance

kek.

I'm pretty sure the gate driver on the DRV8302 failed, the thing is, the digital core of the chip can't detect that so it doesn't output a fault.
```

---
## \#11 Posted by: JensSjogren Posted at: 2019-04-07T09:32:45.779Z Reads: 75

```
Hmm okay, how did you see where it is fried? I'm not at home so i cant look for it closer now. 

I guess this isnt something i just replace with a new chip and soldering iron? 😅
```

---
## \#12 Posted by: Gamer43 Posted at: 2019-04-07T09:40:32.646Z Reads: 64

```
I can't see that it's fried, but based off of your symptoms I can tell that is most likely the case.

You will need a heat gun to remove the old and put on a new DRV8302.
Because you have to reflow solder off the old chip and reflow solder on the new chip because of the exposed ground pad.
```

---
## \#13 Posted by: JensSjogren Posted at: 2019-04-07T09:42:54.859Z Reads: 66

```
So no soldering necessary then? I'll look into that. Thanks for the help! :)
```

---
## \#14 Posted by: Gamer43 Posted at: 2019-04-07T09:43:11.009Z Reads: 70

```
uhhh, more like a tougher time soldering.....
You will have to replace the DRV8302

Thanks exposed ground pad.
```

---
## \#15 Posted by: JensSjogren Posted at: 2019-04-07T12:42:05.240Z Reads: 62

```
This is what i could manage with my phone camera 


![20190407_143440|375x500](upload://zmGY5D134xwb478tx8K4AkF73t2.jpeg) 

![20190407_143234|374x500](upload://nzSEDOuDfCVrAPdqv3SD5O87oaW.jpeg) 

![20190407_143448|375x500](upload://3rSXnsdfPt9WeDTLVcNghCeEzbL.jpeg)
```

---
## \#16 Posted by: Gamer43 Posted at: 2019-04-07T12:54:03.121Z Reads: 60

```
If you have a multimeter, do you think you could try probing across C28, C29, C30, C20, and C52 to see if any of them are shorts?

If there's a short, it's not the capacitor, it's definitely the DRV8302.
```

---
## \#19 Posted by: banjaxxed Posted at: 2019-04-07T13:52:47.355Z Reads: 51

```
Presumably stock heatsink? That is fairly abusive if pushing amps so extremely likely a ‘silent’ drv failure 

You’re lucky to get the advice above, it’s gold
```

---
## \#20 Posted by: Friskies Posted at: 2019-04-07T14:09:30.964Z Reads: 49

```
100 amps per motor is pretty high, I'd say the poor old 8302 is dead thanks to it :frowning:
```

---
## \#17 Posted by: mmaner Posted at: 2019-04-07T14:36:33.045Z Reads: 33

```
2 posts were split to a new topic: [I aquired an esk8 and need help](/t/i-aquired-an-esk8-and-need-help/89702)
```

---
## \#21 Posted by: JensSjogren Posted at: 2019-04-07T14:39:15.399Z Reads: 42

```
well atleast i know the limits of the focbox now.. ;P will be interesting to see if my flipsky 6.6 with alu enclosure can handle it. ripping around on dirt is just to much fun to stop..

thanks for all the tips, i'll check with the multimeter. if it turns out to be the 8302 do we know anyone in the EU that could replace it for a fair amount?
```

---
