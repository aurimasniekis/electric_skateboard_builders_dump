# Dual VESC connected with can - question about damage risk - Is there a way to prevent the risk and still using CAN?

### Replies: 22 Views: 643

## \#1 Posted by: boubak Posted at: 2018-10-07T14:57:43.988Z Reads: 122

```
Hello,

I have a question for the people well versed in the VESC's arts.

In anticipation of connecting two VESC with CAN, I would like to know if there is a risk of damaging one of the VESC if the other goes unpowered accidentally.

And if there's a risk, are all the different VESC versions and brand concerned by this problem ?

Cheers,

Boubak
```

---
## \#2 Posted by: Trdolan03 Posted at: 2018-10-07T14:59:27.655Z Reads: 116

```
Yes, if you plug in only one VESC with a canbus connected it will blow it. I am pretty certain this is universal across brands and hw platforms
```

---
## \#3 Posted by: boubak Posted at: 2018-10-07T15:20:08.548Z Reads: 110

```
@Trdolan03 : Thanks for your answer :slight_smile:

So I have 2 questions : 
*  What will burn ?
*  Is there a way to prevent it happening other that powering both vesc via the same power source (that's more a workaround than a real solution for me)?

Cheers,

Boubak
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-10-07T15:40:17.829Z Reads: 101

```
your best option would be to use a split ppm cable in your circumstances
```

---
## \#5 Posted by: boubak Posted at: 2018-10-07T16:19:18.517Z Reads: 101

```
Thanks for your answer :slight_smile: 

Yes, I already thought about this solution.

But is there a workaround with the use of CAN connection.

I find it weird that this trivial edge case can damage a VESC :confused:, it's a little bit like if it hasn't been really designed to be used with CAN.

I don't intend to be rude, I just don't understand/know the electronical limitations that led to this unmanaged problem. 

So, if somebody with the knowledge of the technical details behind this problem can explain me why, I will be happy :).

Cheers,

Boubak
```

---
## \#6 Posted by: Andy87 Posted at: 2018-10-07T17:43:14.863Z Reads: 92

```
Flipsky 6.6 don’t have this issue anymore.
You can plug in and out your CAN at any time
without to damage the other
```

---
## \#7 Posted by: visnu777 Posted at: 2018-10-07T17:58:12.027Z Reads: 91

```
The same goes for the FSESC 4.12, I did this by accident and nothing happened.
```

---
## \#8 Posted by: boubak Posted at: 2018-10-09T09:19:31.029Z Reads: 89

```
@Andy87 : 

Thanks for your message !
Where did you get this information ? I can't find it anywhere.

@visnu777 : 

Thanks for your message !
A one-time test is not enough to make this statement , do you have other examples ?

@Kug3lis and other electronic engineers here : 

Is there an electronical way of protecting the vesc from this damage ? (putting-a-resistor-somewhere style, but it's just a noob guess from a non electronic engineer :slight_smile:) 


Cheers,

Boubak
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-09T09:32:26.306Z Reads: 86

```
The video isn´t online anymore.
https://www.electric-skateboard.builders/t/eur-group-buy-100-102-vesc-6-6-flipsky/63924/139?u=andy87
maybe @moon can upload it for you once again.
You can see in it how they multiple times connect and disconnect the CAN bus 
while in operation.

The FSESC 4.12 wiil not fit to your needs as the max const. current is below 50A.

You can always get a dual unit, like the FSESC6.6 or Focbox unity.
They have an internal CAN bus, so definitly no way to accidently unplug anything.
```

---
## \#10 Posted by: Jc06505n Posted at: 2018-10-09T09:36:20.296Z Reads: 82

```
Do it the @longhairedboy way. Soldier and hot glue the canbus cable on so it never disconnects and ensure that the vesc’s are connected to the anti spark first before the battery so they turn on simultaneously. Most of the problems just step from the canbus cable disconnecting

edit: he heat shrinks them lie he says below not glue them my fault.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-10-09T09:41:26.610Z Reads: 82

```
what I always wanted to know...
If I make a reboot via VESC tool while connected via CAN, it will also fry the port?
If yes, than the option with soldering all together, plus same power supply plug wouldn´t help :sweat_smile:
```

---
## \#12 Posted by: longhairedboy Posted at: 2018-10-09T10:54:27.149Z Reads: 76

```
you don't HAVE to reboot one at a time. However, rebooting and disconnecting from power aren't the exactly same thing. you can reboot just one from software and nothing should break. But the simplest way to restart them after changes are made is to simply power them both off and back on at the same time. i beleive its the full power cycle that creates the weird voltage difference that causes the can bus to fry, not simply "rebooting" which is akin to restarting without powering off a computer. 

the easiest way is to wire them first, then power them on at the same time, then configure each one without rebooting or powerering down, then power them both off and back on again at the same time. I've done it this way hundreds of times. it works. 

I no longer just use a connector and hot glue it on. I use wire with crimped connectors on them without the connector housing, and i solder them to the pins and heat shrink them with 3mm heat shrink. no glue there, just solder and heat shrink. its easy to remove when you want to, and will not remove itself unless a pin breaks.
```

---
## \#13 Posted by: Andy87 Posted at: 2018-10-09T10:59:28.611Z Reads: 68

```
I know that I don’t have to reboot.
It was just a question as you know, when you sure everything is fail safe you don’t take care, just push the wrong button...instead of disconnect push the reboot and hoobs vesc broken...
So it’s good to know that the reboot will not have the same affect if connected via CAN.
Thx for that 👍
```

---
## \#14 Posted by: Skunk Posted at: 2018-10-09T11:01:49.918Z Reads: 65

```
[quote="longhairedboy, post:12, topic:70441"]
I use wire with crimped connectors on them without the connector housing, and i solder them to the pins and heat shrink them with 3mm heat shrink. no glue there, just solder and heat shrink. its easy to remove when you want to, and will not remove itself unless a pin breaks.
[/quote]

Bookmarked & Copy n paste into by "what the hell am i doing " folder.
Putting my board together in the next week.  Good info to have.
```

---
## \#15 Posted by: Wraith Posted at: 2018-10-09T11:55:01.244Z Reads: 63

```
Glad i read this thread. You may just have saved me a couple of $$$ worth of vesc repairs/replacements :laughing:
```

---
## \#16 Posted by: lrdesigns Posted at: 2018-10-09T14:45:41.351Z Reads: 56

```
[quote="longhairedboy, post:12, topic:70441"]
I use wire with crimped connectors on them without the connector housing, and i solder them to the pins and heat shrink them with 3mm heat shrink. no glue there,
[/quote]

This method sounds legit. But I’d still put hot glue on top for extra peace of mind. Would make maintenance more painful though.
```

---
## \#17 Posted by: visnu777 Posted at: 2018-10-10T09:13:24.232Z Reads: 51

```
[quote="boubak, post:8, topic:70441"]
A one-time test is not enough to make this statement , do you have other examples ?
[/quote]

It happened at least twice, of course that's not representative but I won't force it since I already burned enough money with VESCs (all my stupidity)
```

---
## \#18 Posted by: boubak Posted at: 2018-10-10T09:36:29.884Z Reads: 50

```
Haha, I wasn't asking you to burn multiple vescs for the sake of the test :smiley:
```

---
## \#19 Posted by: boubak Posted at: 2018-10-11T09:20:48.341Z Reads: 42

```
@Andy87 : 

Thanks for the informations :slight_smile: ! 

[quote="Andy87, post:9, topic:70441"]
maybe @moon can upload it for you once again.
You can see in it how they multiple times connect and disconnect the CAN bus
while in operation.
[/quote]

But wasn't the burning problem that it's when one VESC goes off and not when the can cable is disconnected?

Is there a risk to burn a VESC if I unplug the CAN cable without unpowering one of the VESC , too?

[quote="Andy87, post:9, topic:70441"]
You can always get a dual unit, like the FSESC6.6 or Focbox unity.
They have an internal CAN bus, so definitly no way to accidently unplug anything.
[/quote]

 Yes, True, but I don't like Focboxes
and about the dualafter what said @Kug3lis and other protagonist about the possible crappy quality of these VESCs, I don't totally trust this brand.

@Kug3lis : Could you possibly explain with facts why these VESC are not good ?

@longhairedboy :  Thanks for sharing your method :slight_smile:

Cheers,

Boubak
```

---
## \#20 Posted by: Vanarian Posted at: 2018-10-11T09:44:27.201Z Reads: 37

```
FOCBOX unity are no VESC anymore AFAIK, Fsesc6.6 dual are still VESC so it's a no Brainer :v:

Edit : Seems I was wrong, Unity does indeed runs Vedder's firmware!
```

---
## \#21 Posted by: Jc06505n Posted at: 2018-10-26T17:16:35.493Z Reads: 23

```
[quote="Vanarian, post:20, topic:70441"]
FOCBOX unity are no VESC anymore AFAIK
[/quote]

[quote="Deodand, post:62, topic:64944"]
Enertion has made the leap into **fully custom open-source vesc-based firmware** to accompany their hardware
[/quote]

10 character
```

---
## \#22 Posted by: Vanarian Posted at: 2018-10-26T19:53:29.770Z Reads: 17

```
Can you confirm the Focbox **Unity** runs on Vedder's based software, and is compatible with VESC-Tool and all its features?

Edit : It is stated too on product page on enertion website. Nice!
```

---
