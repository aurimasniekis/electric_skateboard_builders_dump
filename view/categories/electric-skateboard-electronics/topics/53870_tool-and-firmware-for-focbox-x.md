# Tool and Firmware for Focbox X

### Replies: 12 Views: 589

## \#1 Posted by: ksfacinelli Posted at: 2018-04-29T19:26:28.389Z Reads: 156

```
Hi I was interested in understanding what tool and firmware users of Focbox -X are using and why?

BLDC Tool?, Ackmanic, Vesc Tool? Also what firmware have you installed?

Thanks in advance,

Kevin
```

---
## \#2 Posted by: Scoo_B_SK8 Posted at: 2018-04-29T21:33:48.044Z Reads: 146

```
[quote="psychotiller, post:2, topic:53876, full:true"]
Use the 2.18 bldc tool and call it a day. no firmware updates required.
[/quote]

[quote="Deckoz, post:3, topic:53876, full:true"]
What @psychotiller said. 2.18 and go. Should be fine. I’ll take a look. Out n a group ride and just watched a guy get taken away in an ambulance so… I’ll have to check it later.
[/quote]


hows that build coming?
```

---
## \#3 Posted by: psychotiller Posted at: 2018-04-29T21:38:24.002Z Reads: 135

```
Which one? working on 4 builds today lol
```

---
## \#4 Posted by: Bjork3n Posted at: 2018-04-29T22:22:07.179Z Reads: 116

```
I Use Ackmaniac 3.100 FW on my focboxes.
Why? Cuz its the best freaking FW for an esk8.

Never going back to stock FW or any other that aint using wattmode.
```

---
## \#5 Posted by: ksfacinelli Posted at: 2018-05-02T15:41:56.956Z Reads: 75

```
Bjor3n,

I have used Ackmaniac as well as setup FOC control, can you provide details on wattmode or direct me to a discussion, NEWBY.

Kevin
```

---
## \#6 Posted by: ksfacinelli Posted at: 2018-05-02T15:46:50.302Z Reads: 68

```
Also waiting on arrival of hall sensor cable to hook up TB 6437 190kv dual motor,  the configuration I have with 10p5s requires the board to have a little shove to get moving....I would like a smoother start from standing acceleration.  Is there a setting to tweak outside of the motor wizard and Input wizard setting to refine sensor less FOC.

Thanks,

Kevin
```

---
## \#7 Posted by: Deckoz Posted at: 2018-05-02T15:53:24.600Z Reads: 63

```
Not really. You need sensors.

When the motor is sensorless, and not moving or moving at a slow rate there is not enough Back EMF voltage to let the controller understand where the motor is at in rotation relative to the phases.

So sensors... Or push start sensorless.
```

---
## \#8 Posted by: Bjork3n Posted at: 2018-05-02T16:18:46.358Z Reads: 58

```
Im no expert but i can tell you that the stock fw was no good for me.
With ackmaniac i was able to accelerate fast out of corners with full control.
The remote now does exactly what i tell it to do, before with stock fw it was more like a on/off switch when i accelerated.

Im running bldc and sensorless.
```

---
## \#9 Posted by: ksfacinelli Posted at: 2018-05-02T16:20:09.300Z Reads: 55

```
I will try setting up BLDC mode and see what the difference from FOC is...
```

---
## \#10 Posted by: ksfacinelli Posted at: 2018-05-02T16:21:17.612Z Reads: 55

```
Thank you for the response will install sensors when they come,  do you run BLDC or FOC sensored?
```

---
## \#11 Posted by: Bjork3n Posted at: 2018-05-02T16:22:13.558Z Reads: 53

```
From what i know FOC is smoother and more quiet.
BLDC is not as nice as FOC, but i use BLDC just to keep things safe. 

And i like the bldc sound , its great to make people move out of my way :)
```

---
## \#12 Posted by: Deckoz Posted at: 2018-05-02T17:14:12.872Z Reads: 41

```
I run FOC sensored...
```

---
