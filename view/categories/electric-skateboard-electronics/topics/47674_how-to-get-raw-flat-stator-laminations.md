# How to get raw flat stator laminations?

### Replies: 22 Views: 1151

## \#1 Posted by: Vanarian Posted at: 2018-02-27T18:05:52.751Z Reads: 144

```
Silly me wants to cut laminations out of a stator I salvaged without damaging them lams... and I have no clue how I'm supposed to proceed.

I realize that it is steel, which is stronger than aluminum which has given me a headache already when cutting it with domestic tools. 

Else another question I got is  : where could I buy / retrieve straight lams cut ? 

Do you guys have good addresses for cheap thin steel lams ?
```

---
## \#2 Posted by: barajabali Posted at: 2018-02-27T18:07:53.788Z Reads: 141

```
Technically you can use a solid stator instead of laminations but it just won’t be as strong as a laminated stator. In terms of motor strength. But it could work as a proof of concept if you’re testing your motor.
```

---
## \#3 Posted by: Hummie Posted at: 2018-02-27T18:10:47.119Z Reads: 135

```
you can split stators pretty easily if you're splitting horizontally

a solid stator would be "stronger" in that it could produce more maximum torque as there will be a bit more iron there so it can hold a stonger magnetic field, but it will got hot from eddy currents as it switches polarity
```

---
## \#4 Posted by: Vanarian Posted at: 2018-02-27T18:12:47.238Z Reads: 128

```
When you say horizontal, do you mean splitting between lams "layers" (parallel to lams) or do you mean cutting a pole itself (perpendicular to lams) ?
```

---
## \#5 Posted by: Hummie Posted at: 2018-02-27T18:13:24.870Z Reads: 115

```
taking the lams apart at their seams.  splitting between them.  Ive done that and it's not hard
```

---
## \#6 Posted by: Vanarian Posted at: 2018-02-27T18:14:01.897Z Reads: 109

```
How did you proceed ? If possible i wanna try not to chip them too much
```

---
## \#7 Posted by: Hummie Posted at: 2018-02-27T18:16:04.151Z Reads: 104

```
use a blade.  the danger isn't chipping, the stuff will bend,  ....the real danger is when you go to reinsulate the stator so you can wind it again without shorting through it.  get the right insulation and do it right..  cover all the sharp corners with the right stuff or it will be a nightmare.  ive had that nightmare
```

---
## \#8 Posted by: Hummie Posted at: 2018-02-27T18:18:46.604Z Reads: 95

```
or..  another way would be to make a powdered core stator and you could even make that from possibly beach sand and glue.  the goal being to get as much iron in as possible.  you wont get as much as a laminated stator but it can be pretty good and with the powder and glue you can chose the shape.  
a hard mold and you'd have to press the resin filled powder in.  never done it though.
```

---
## \#9 Posted by: Vanarian Posted at: 2018-02-27T18:22:18.124Z Reads: 89

```
Ok thanks for the tips ! I should try that first (hope to get some successful result) else I'll try the iron powder resin ; might be a good way to experiment with that.
```

---
## \#10 Posted by: Deckoz Posted at: 2018-02-27T18:47:57.672Z Reads: 82

```
I'm confused as to why you need to split the laminations? Typically they are welded down the spines...

Why not just laser cut your own laminations?
```

---
## \#11 Posted by: Hummie Posted at: 2018-02-27T19:05:31.312Z Reads: 84

```
ive never come across a stator that was welded and they've all been easy to peel apart.  I've peeled them apart to take a bit off when there isn't enough room for the stator in the motor.  how rare is a laser cutter that can do laminations at .2mm or .35mm?
```

---
## \#12 Posted by: Deckoz Posted at: 2018-02-27T19:10:07.860Z Reads: 79

```
Why do you want thicker lams?

Thinner lams will give more power and more stable Eddy currents. And how else would you electrically connect the lams? They're welded and then grinded Down so they're tacked.
```

---
## \#13 Posted by: Vanarian Posted at: 2018-02-27T21:15:42.482Z Reads: 69

```
Where do you laser cut them? I need tiny flat rectangles cut from both long sides.something like 30x4mm
```

---
## \#14 Posted by: Deckoz Posted at: 2018-02-27T21:43:28.896Z Reads: 69

```
What? I'm so confused what your trying to accomplish.

A stator is a bunch of layers with the poles cut into the sheets. Stacked up welded together. Coated with epoxy and wound.

![winding|355x280](upload://okVYxy5Np6JzKY9HGwqgXo6DC89.png)

What are you going to do with rectangular laminations? We're you trying to just make the poles? You need to wind perpendicular to the laminations...

I'm honestly confused what you are trying to achieve
```

---
## \#15 Posted by: Vanarian Posted at: 2018-02-27T22:45:04.294Z Reads: 59

```
Trying to create a 63mm Frankbrushtein abomination stuffed with axial magnets and axial laminations on top of the existing radial design. With big ass 18awg wiring too. 

I want to test how the Frankbrushtein hybrid fares against a "normal" counterpart (sk3, APS...), experiment on the rolling drag, if there is significant added torque or just a waste of experiment. But it's going to be fun so hell Yea it I'll be worth it anyway.

So even better I'd need some "T" like lams else I'm gonna epoxy glue it on the wiring and call it **alive**!
```

---
## \#16 Posted by: Hummie Posted at: 2018-02-28T00:04:55.574Z Reads: 54

```
stators are normally cut then stacked with glue to hold them together having them ideally electrically isolated from each other.  never heard of them welded together.  seems unnecessary.

@vanarian if youre going to add an axial magnetic interface using a typical outrunner and then add magnets and iron...I think it might not be well supported with the way a standard outrunner has only support on one side but maybe be ok.    
but can you bend the magnetic field?  you'd be having a magnetic field as with a typical outrunner and the polarity would be facing straight out from the tooth, the direction the coils are circling, but can you bend the field by having a stator with overhanging teeth at the top and bottom of the stator and get the field to bend in that direction following the iron?  ive seen similar and think you can, and we don't do it because hard to manufacture a stator that way

if youre trying to get the most torque for a given size you could do the same outrunner radial design and get cobalt laminations maybe.  holds a stronger magnetic field before saturation than electrical steel.  probably kinda expensive to get made and poisonous if you do it yourself but 25% more torque before saturation.
http://www.vacuumschmelze.com/fileadmin/Medienbiliothek_2010/Forschung___Innovation/Publikationen/Volbers_Gerster_-_High_Saturation_High_Strength_Iron-Cobalt_Alloy_for_Electrical_Machines.pdf
you've probably read.  ..
```

---
## \#17 Posted by: Deckoz Posted at: 2018-02-28T00:34:28.330Z Reads: 52

```
[quote="Hummie, post:16, topic:47674"]
stators are normally cut then stacked with glue to hold them together
[/quote]

Lol I've never seen this. 

But gluing and cleating make weak motors. 

Thin laminations, pressed and welded, wound with the thickest guage possible, with n52sh arc magnets will make a motor with substantially more powerful then the same or thicker laminations that are welded or glued and cleated.
```

---
## \#18 Posted by: Hummie Posted at: 2018-02-28T00:52:28.008Z Reads: 53

```
talking of the stator alone when you say a stator with thinner laminations will make more power yes because will have less eddy current.  the benefit of the thin lams being the iron of the stator is more electrically isolated,  even better in a way would be the powder core stator where eddy currents have very little room to travel as the conductive pathways are as short as dust particles, but it's the same scenario with the powder core and the thin lams..great in reducing eddy currents but less actually iron as it's been replaced by glue between laminations or glue between iron dust to electrically isolate.  the motor with the thinnest laminations will create more power at high speed and low torque while a motor with thicker lams could potentially have more power at slowest speeds as it would be able to have more torque before saturation.   if you have a stator with the thinnest lams and 75% iron and 25% glue vs a thick lam stator with 85% iron and 15% glue...and you try to get the most power out of it on the steepest hill...the one with less stator has less maximum torque potential before saturation and if you kick it too many amps it will go over 1.7 tesla magnetic field maximum of the steel and it will fall off cliff into heat with amps beyond.  that's a scenario where thicker lams could be more power and it could be dramatic but generally yea thinner is better.  but welded...maybe they do it on cheaper stators but it would reduce the isolation of the laminates which is the point of laminates.   cleated?  I think you mean to orient the laminations together with each other in the stack

but I read they do both welding and gluing.  I'm betting gluing will produce a more powerful motor with less eddy currents.
```

---
## \#19 Posted by: Deckoz Posted at: 2018-02-28T02:28:39.167Z Reads: 47

```
Cleating is using metal straps...

https://www.youtube.com/watch?v=g4MGXuuk00A

...lol
```

---
## \#20 Posted by: Hummie Posted at: 2018-02-28T02:43:38.581Z Reads: 43

```
that is funny I guess  if you think machines are funny
```

---
## \#21 Posted by: Vanarian Posted at: 2018-02-28T17:26:34.132Z Reads: 34

```
Hard to tell if I can bend the magnetic field, but I've been guessing that crossing the axial and radial flux should not be a problem if polarities are lined up. If it works this would also be a way to reduce end-turns wasted power.
```

---
## \#22 Posted by: FullMetal_Machinist Posted at: 2019-01-20T21:57:34.234Z Reads: 18

```
If you want to make a horizontal motor for the inline skates the easiest way would be to take a toroidal transformer of apropriate size (something like 60 to 150 watts depending on wheel size), remove the winding and cut horizontally into the laminations with an angle grinder to make slots for the winding.
It wont be preety but will do for a proof of concept. Avoid overheating the laminations, best do it wet.
Done that once for wind generator and it worked.
```

---
