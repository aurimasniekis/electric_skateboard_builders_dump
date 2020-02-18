# First build wiring diagram, please triple check it :)

### Replies: 22 Views: 463

## \#1 Posted by: Lobap Posted at: 2019-02-17T22:52:44.209Z Reads: 112

```
Hola everyone,

I'm terrified to burn up my house so... could someone take a look over my wiring diagram? :slight_smile: I already bought a fire extinguisher spray and a fireproof blanket, just in case...

I have finished the connections today... Following is the current status with some stickers to explain where the wires come from/go to, hope you understand. 

![image|1190x410](upload://clflEPtyDUhAvHICE01HOdIjobj.jpeg)  


This is what I draw.... like a year ago, and it's finally done!

![image|690x460](upload://21My4DXd8C8GaU6yJNilkGHsy3b.jpeg) 

A couple of questions:
- The positive wire that goes to the charge port, I soldered it to the bullet connector that goes plugged to the antispark, is that ok? shall I solder it straight to the XT90 that comes from the battery or its the same thing? 
- I sent my SpaceCell to a friend to swap the balance wires connector to the right one that matches the BMS connector (Enertion one was bigger), but he had to also invert the position of the wires to match the diagram. The thing is, I'm not sure he actually did the wire position invert or he just solder it as it came. If I connect the battery and the BMS and the position is not swaped, what can go wrong? :blush:
- Once I'm sure everything is ok... shall i connect first the balance wires connector then the XT90, or the other way around? 

Thank you in advance!

Cheers,
Pablo
```

---
## \#2 Posted by: Psmrman90 Posted at: 2019-02-17T23:13:47.258Z Reads: 97

```
I'm not amazing at wiring, but without a canbus connecting the two vescs, you'll need two Bluetooth modules to monitor both vescs
```

---
## \#3 Posted by: Lobap Posted at: 2019-02-17T23:26:53.806Z Reads: 93

```
The green thing is supposed to be the CANBUS connection!
```

---
## \#4 Posted by: banjaxxed Posted at: 2019-02-18T00:01:12.727Z Reads: 90

```
Seems ok to me, the diagram seems to have a wiring mistake for the y split to the focboxes but the picture is ok
```

---
## \#5 Posted by: b264 Posted at: 2019-02-18T00:04:43.351Z Reads: 90

```
Put a fuse on the charge port negative

https://www.mouser.com/ProductDetail/576-099707.5WXN
```

---
## \#6 Posted by: b264 Posted at: 2019-02-18T00:09:06.074Z Reads: 87

```
[quote="Lobap, post:1, topic:84487"]
The positive wire that goes to the charge port, I soldered it to the bullet connector that goes plugged to the antispark, is that ok? shall I solder it straight to the XT90 that comes from the battery or its the same thing?
[/quote]

It's the same thing

[quote="Lobap, post:1, topic:84487"]
I sent my SpaceCell to a friend to swap the balance wires connector to the right one that matches the BMS connector (Enertion one was bigger), but he had to also invert the position of the wires to match the diagram. The thing is, I’m not sure he actually did the wire position invert or he just solder it as it came. If I connect the battery and the BMS and the position is not swaped, what can go wrong? :blush:
[/quote]

The BMS will become broken

[quote="Lobap, post:1, topic:84487"]
Once I’m sure everything is ok… shall i connect first the balance wires connector then the XT90, or the other way around?
[/quote]

~~Balance first~~ see below
```

---
## \#7 Posted by: Lobap Posted at: 2019-02-18T20:43:25.127Z Reads: 60

```
Something like that, right?

![image|500x500](upload://7A2Y3f0QAebEju9h4S0lNmH54ro.jpeg) 

How many amps? Thanks a lot!
```

---
## \#8 Posted by: Lobap Posted at: 2019-02-18T20:45:17.001Z Reads: 59

```
Ok, thanks a lot for your answers.

I think I need a multimeter to check the balance wires before I can plug anything safely....
```

---
## \#9 Posted by: Lobap Posted at: 2019-02-18T20:47:50.420Z Reads: 59

```
Thanks man.

Which mistake do you see in the Y split? If you check the pic, next to the bottom of the nice green CANBUS cable you sent me, there are 2 XT60 connectors going below the velcro stripe and then there is the Y connector joining them to the antispark.

Is that ok?
```

---
## \#10 Posted by: Sebike Posted at: 2019-02-18T20:56:35.452Z Reads: 57

```
[quote="b264, post:6, topic:84487"]
> Once I’m sure everything is ok… shall i connect first the balance wires connector then the XT90, or the other way around?

Balance first
[/quote]


Not familiar with whatever BMS is used here, but often it's the other way around. First connect the main leads and then the balancing leads, or BMS will fry. You sure this is the order this should be connected @b264 ?
```

---
## \#11 Posted by: b264 Posted at: 2019-02-18T21:06:06.983Z Reads: 52

```
No, I attach them to the inside and solder onto them.  But one of those would work just fine.
```

---
## \#12 Posted by: b264 Posted at: 2019-02-18T21:06:25.015Z Reads: 55

```
Nope, not sure.
```

---
## \#13 Posted by: pat.speed Posted at: 2019-02-18T21:07:50.454Z Reads: 55

```
Yes, it is always the b- first. Unless your balance leads have b- included.

@Lobap to check the wiring of the balance wires you need to use a multimeter and check which one is the first cell. The order of voltage should increase by about 4v each time you move to the next pin.

If the wiring is correct it the first wire (the 4v one) will plug into the bms side marked either b- or b1. It should say on the bottom near the connector which pin is for which cell. After that they should all just increase as normal
```

---
## \#14 Posted by: banjaxxed Posted at: 2019-02-18T21:22:39.536Z Reads: 49

```
yeah don't worry the polarity and connection in real life is fine as far as I can see
```

---
## \#15 Posted by: Lobap Posted at: 2019-02-18T22:01:13.416Z Reads: 47

```
Oks, will take the following, 7.5A then? This one comes with 30A, will work straight away or do I need exactly a 7.5A fuse? 

https://www.amazon.es/Neuftech%C2%AE-Portafusible-impermeable-incluyendo-fusible/dp/B00UX6NIQE/ref=sr_1_17?dd=Esi7A1o8eT7TP7WYBsc4zQ%2C%2C&ie=UTF8&qid=1550527026&sr=8-17&keywords=fusible&refinements=p_90%3A6820340031&th=1
```

---
## \#16 Posted by: Lobap Posted at: 2019-02-18T22:01:47.999Z Reads: 45

```
Yup, many thanks, tomorrow i will pick a voltimeter and check it as you described :slight_smile:
```

---
## \#17 Posted by: b264 Posted at: 2019-02-18T22:05:35.065Z Reads: 45

```
I would just solder one of these $0.67 fuses in and be done

https://www.mouser.com/ProductDetail/576-099707.5WXN
```

---
## \#18 Posted by: b264 Posted at: 2019-02-18T22:06:10.160Z Reads: 45

```
By the way, your avatar

So much :heart:

I actually like that one a lot.  I know a lot folks thought it was crap, but not me.
```

---
## \#19 Posted by: Lobap Posted at: 2019-02-20T13:35:24.778Z Reads: 31

```
Fuse adaptor ready, I guess for my 10s4p (Samsung 30Q from the Raptor) I need a **15A fuse** (16A max charge current), right? 

![image|245x335](upload://sCIhrJB2EEiSIk4IeOsGwE4WpYv.jpeg) 

Just one step to finish: enclosure holes & aligning them with the encosure bolts... real PIA :frowning:
```

---
## \#20 Posted by: b264 Posted at: 2019-02-20T20:36:27.341Z Reads: 26

```
Just double whatever maximum charge current you'll be using.  I use these for 1A, 2A, and 4A charging

https://www.mouser.com/ProductDetail/576-099707.5WXN
```

---
## \#21 Posted by: Mudders Posted at: 2019-02-20T20:48:12.365Z Reads: 25

```
Why the negative? Does it matter?
```

---
## \#22 Posted by: b264 Posted at: 2019-02-20T20:50:09.788Z Reads: 25

```
Can be either one, but the way BMSs work, it's easiest to not make any mistakes if you just connect every positive in the whole system together.  And put all the loop keys and fuses and stuff on the negative.  Since the BMS forces it anyway for a portion of the wiring.

Instead of having the "common" be negative on part of the system and positive on the other part... the way BMS work... just easier to use positive as "common"
```

---
