# Not sure if you have shorted phase wires? Here is how to test them without frying your ESC

### Replies: 9 Views: 481

## \#1 Posted by: Andy87 Posted at: 2018-12-22T08:23:15.537Z Reads: 117

```
A while ago I shorted 3 of my motors because the mounting screws where 1mm too.
Due to vibrations the screws rub off the isolation and than shorted the phase wires to each other via the motor case.
I measured the resistance from the mounting hole to the phase wires like this
![image|504x500](upload://vR0jQGEYfQbAvTsPfwmeeEeC8Qy.jpeg) 
What gave me 0 ohms, so a full short.
I thought I can easy fix it by just adding a piece of heat shrink over the wires, but there is no way to get it there without to take off the top part of the stator. As this part is usually glued in it’s pretty much not possible without proper tools.
(Or as min not for me as noob 😅)
I first tried to cover the damaged part of the wire with liquid tape, what worked out, but I wasn’t super happy with it.
I decided to make that thing bullet proof by epoxy the phase wires all over the place where they where damaged.
That looked now way much better, but the question was, 
how to double check if really all damaged parts of the isolation now covered?
Sure you can just spin it up with your ESC but with it you risk to fry one more controller.
So how to do it without? 🤔
Our outrunner produce a specific current and voltage when spinning (regenerativ breaks), so if all phase wires are ok, than the voltage produced while spinning should be the same for all three wires, right?
Right, and here is the most easy way to check that.
You need your motor on the motor mount
You need a drill
And you need a multimeter set to AC voltage
![image|375x500](upload://oa4MnH4eMZFU90v50uMfNgvq67a.jpeg) 

Connect your multimeter first to phase A and B
Than connect the drill to your motor shaft
Spinn up the motor with the drill
Check the voltage on your multimeter and remember what was displayed 
Than move on and connect the multimeter to phase A and C 
Spinn up the motor again
The voltage reading should be the same now
If yes move on and connect your multimeter to
Phase B and C
Same test, same result.

If in all three cases the indicated voltage is the same, you good to go and can use your motor like before.
```

---
## \#2 Posted by: linsus Posted at: 2018-12-22T09:37:05.004Z Reads: 105

```
Its usually not so hard to dissasamble the motor as one would think. But as you stated, since the copper in the motor is lenz wires, re-laminating is the way to get proper isolation again if the short is inside the motor. Also good to check for forther damage this way. (cleaning the motor is usually key to keep it functioning many years as well)

The generator test is pretty clever. Another reading is the actual resistance in respective phases. They should be similiar or atleast very close. (mOhm). Could be a worthy double check.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-12-22T11:51:41.729Z Reads: 86

```
It’s not hard to take off the bell and it’s also not hard to remove the bearings, but to come to the place where my phase wires where broke you need to dismount also the front part (where the screws sit in)I tried to get it off, but in my case it wasn’t possible. I tried it with heating up the inner part, but that doesn’t help too and I didn’t want to use more heat as it’s possible to meld down the isolation of the windings.
```

---
## \#4 Posted by: linsus Posted at: 2018-12-22T11:57:37.601Z Reads: 82

```
Scary, What motor was that? :D ill make sure to never buy it. 
Dissasambled jacob hubs, hummie first hubs and mad hubs, sk3, sk8 and alien motors so far. no problems yet :P
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-22T12:02:44.637Z Reads: 77

```
That already too late for you 😅
You already bought alien motors 😜
They where the aps 6384 motors.
Let me please know for future, how you got the red part of the blue part?
![image|374x500](upload://nqwIY3cLWYahZBCVACCc4c4C4Ct.jpeg)

I took the bearings out, but I couldn’t press the inner part out of the outer part.
Even not with heat.
```

---
## \#6 Posted by: linsus Posted at: 2018-12-22T12:05:34.139Z Reads: 66

```
was maybe a year ago i opened em. Cant remember having any struggle they're 6374 aliens tho.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-12-22T12:07:57.584Z Reads: 63

```
I think it is one solid piece is it not? 

If it’s not you should try heating the outer most part not the inner one as heat makes things expand and you want the outer piece looser not the inner tighter
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-22T12:11:22.867Z Reads: 61

```
No it’s two parts.
I was speaking with aps too about it.
It should be possible to take this two parts out of each other. I know that others did that before already.
The thing is that the parts wher not only put together inside, they where also fixed with epoxy.
I tried only one motor, maybe with the others it would have been different, but I don’t think so.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-12-22T12:13:17.476Z Reads: 58

```
In mine the inner part was glued to the part where the windings on.
I also didn’t have had a tool in the right diameter to press the inner part out.
What you used for it?
I have seen people using parts of a flash light for it 😅
```

---
