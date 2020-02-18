# Shorted my motor \[phase?\] leads. Dead VESC. Concerns?

### Replies: 9 Views: 613

## \#1 Posted by: skelstar Posted at: 2018-03-28T23:31:19.439Z Reads: 134

```
So despite having been an electronics technician in a previous life I neglected to make sure that the phase wires weren't going to rub against the motor and eventually short out. It took a few months!

As soon as I got home and tried connecting the VESC to my computer I realised that I had in fact killed the VESC (i.e. the USB controller/hub wasn't working).

I have a replacement VESC, **but I shouldn't have anything to worry about when i try hooking it up again should I**?

(note: I have replaced/repaired the phase wires too)
```

---
## \#2 Posted by: FabianOdermatt Posted at: 2018-03-29T16:20:52.742Z Reads: 112

```

[quote="skelstar, post:1, topic:50504"]
I have a replacement VESC, but I shouldn’t have anything to worry about when i try hooking it up again should I?
[/quote]

I don't think so. But just to be sure, you could measure the ohms between the phase wires. Do you have some kind of multimeter?
```

---
## \#3 Posted by: skelstar Posted at: 2018-03-29T16:42:59.340Z Reads: 101

```
I do. I did, but the resistance between the coils/phases will be super low, given that lots of amps go through them.

I realised this after I measured them of course :)
```

---
## \#4 Posted by: FabianOdermatt Posted at: 2018-03-29T16:55:10.675Z Reads: 89

```
Right, but are they at the same value?
```

---
## \#5 Posted by: skelstar Posted at: 2018-03-29T17:09:18.856Z Reads: 83

```
The values are so low that the errors in my multimeter are more significant.

Less than an ohm.
```

---
## \#6 Posted by: FabianOdermatt Posted at: 2018-03-29T17:24:12.435Z Reads: 77

```
Well I'm not an expert in BLDC motors, but I think this sould be ok. :smiley:
```

---
## \#7 Posted by: Silverline Posted at: 2018-03-29T17:35:01.196Z Reads: 77

```
Yes you can't use a standard multimeter. Buy a cheap LC meter from eBay... If you have a bad winding in the motor, after your accident , you wil most likely kill one of the fet's on the vesc, first time you put load on the motor again. The cheap LC meter, have saved me several times on my racing quads.
```

---
## \#8 Posted by: evoheyax Posted at: 2018-03-29T21:30:10.667Z Reads: 64

```
You need to check with an inductance meter. You should get the same number from all three phase combinations. That tells you the motor is not shorted.

If you get different numbers, it's shorted.

For checking our winds when assembly hummie hubs, we use this little guy:

https://www.amazon.com/KNACRO-Precision-Inductance-Capacitance-Accuracy/dp/B06XSD9VN1/ref=sr_1_6?ie=UTF8&qid=1522359019&sr=8-6&keywords=inductance+meter&dpID=41bh3OXsZZL&preST=_SX300_QL70_&dpSrc=srch
```

---
## \#9 Posted by: skelstar Posted at: 2018-03-30T02:56:10.929Z Reads: 44

```
Thanks for replies, guys.

Agreed re: inductance metre.

I ended up just plugging it in and it works fine (on the bench). Will be taking it easy initially but I'm sure it will be fine.

I'll be sure to wrap/secure my cables so this won't happen again that's for sure.
```

---
