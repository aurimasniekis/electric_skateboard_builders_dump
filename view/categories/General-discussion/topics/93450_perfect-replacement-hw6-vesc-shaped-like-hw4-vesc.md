# Perfect replacement! Hw6 vesc shaped like hw4 vesc

### Replies: 15 Views: 333

## \#1 Posted by: YUTW123 Posted at: 2019-05-11T04:35:01.639Z Reads: 127

```
![SmartSelect_20190511-122229_QQ|690x463](upload://1QB1t1WXbxMIi8YlomhKtMamf8r.jpeg) ![SmartSelect_20190511-122214_QQ|690x437](upload://aKp84Ei819TFaAvmDBiGUda4NL4.jpeg) 

https://www.ebmakers.com/products/perfect-replacement-v6-hardware-is-a-perfect-replacement-for-v4-same-size-same-interface
```

---
## \#2 Posted by: dareno Posted at: 2019-05-11T04:43:44.464Z Reads: 122

```
Unclear body.  Are you sure its a complete sentence?
```

---
## \#3 Posted by: Andy87 Posted at: 2019-05-11T04:47:24.969Z Reads: 119

```
Changed the titel to what I hope is the intention of this thread
```

---
## \#4 Posted by: YUTW123 Posted at: 2019-05-11T04:49:29.145Z Reads: 115

```
hahaha，     Can you write a reasonable title for me?
```

---
## \#5 Posted by: dareno Posted at: 2019-05-11T04:49:58.897Z Reads: 114

```
Is that it my friend?
```

---
## \#6 Posted by: Andy87 Posted at: 2019-05-11T04:50:32.140Z Reads: 112

```
Already done.

What’s with the capacitors for the pcb?
```

---
## \#7 Posted by: SeanHacker Posted at: 2019-05-11T04:51:49.794Z Reads: 112

```
[quote="YUTW123, post:4, topic:93450"]
Can you write a reasonable title for me?
[/quote]

I can... :face_with_hand_over_mouth:
```

---
## \#8 Posted by: YUTW123 Posted at: 2019-05-11T04:55:26.433Z Reads: 107

```
V4 size, V6 hardware.      ＼\ ٩( ᐛ )و /／
```

---
## \#9 Posted by: Grozniy Posted at: 2019-05-11T06:44:04.201Z Reads: 96

```
This is all very nice but where are real world stress tests?
```

---
## \#10 Posted by: Gamer43 Posted at: 2019-05-11T07:14:34.697Z Reads: 88

```
Looks good, but please at least use the ipb014n06n (drop in replacement) instead of those shitty MOSFETs from International Rectifier.
```

---
## \#11 Posted by: banjaxxed Posted at: 2019-05-12T11:12:22.242Z Reads: 56

```
@Gamer43 this is an interesting point on cheap components Vs quality components, would you happen to know which Vendors are using quality components looking at the various PCBs that have been posted up on here?

Of course it affects production price but at a cost of durability & maybe safety too
```

---
## \#12 Posted by: Gamer43 Posted at: 2019-05-12T11:32:17.819Z Reads: 52

```
As long as the part comes from a large, world renowned semiconductor manufacturer, the quality is guaranteed as long as the part is genuine (from reputable distributor such as digikey, arrow, avnet, mouser, farnell, etc.). I'm just harping on the IR MOSFETs because their electrical characteristics suck compared to (cheaper) MOSFETs on the market such as ones from ON Semi and Infineon's OptiMOS series. This is why 4.12 hardware gets so hot running FOC; the switching losses are really high.

However, since IR has become such a big brand, there are actually quite a few fakes on the market; I've been burned by a few. I was actually burned by defective MOSFET drivers from IR that I ordered off Arrow.
```

---
## \#13 Posted by: banjaxxed Posted at: 2019-05-12T11:33:59.660Z Reads: 51

```
The directFETs are ok or are they now copied? Afaik fake DRVs are omnipresent, presumably MCUs too. I don’t really know what I’m talking about in this area but would be interested to know who is using the real stuff besides Trampa

I’m knee deep in focboxes and wondering if they have sourced the best components or ones which balance price point, same question on the Unity
```

---
## \#14 Posted by: Gamer43 Posted at: 2019-05-12T16:13:11.795Z Reads: 37

```
@banjaxxed

99.9% certain directFETs are genuine. The issue 
with directFET is the electrical characteristics are inferior compared to cheaper MOSFETs on the market (compare TPW1R306PL and NTMFS5C604NL for example, or even IPB014N06N). Not exactly sure why Vedder speced IR fets. They are really rugged though, hard to popcorn an IR fet, but thats about the only thing they have going for them.

Basically, when you buy International Recifier, you're paying for the brand and some avalanche ruggedness. Really smart of Infineon to buy them. Especially since Infineon had been making superior MOSFETs years before with similar avalanche ruggedness anyway XD.

Unity uses fets from vishay or nxp I think, much better speced for price point and power dissipation in general, but there is room for improvement.
```

---
## \#15 Posted by: banjaxxed Posted at: 2019-05-12T21:48:44.132Z Reads: 22

```
Thanks for this info @Gamer43 it’s scarce and you obviously know your stuff
```

---
