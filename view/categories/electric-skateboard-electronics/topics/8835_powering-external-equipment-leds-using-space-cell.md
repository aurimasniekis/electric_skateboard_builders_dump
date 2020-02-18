# Powering external equipment (LEDs) using Space Cell

### Replies: 11 Views: 906

## \#1 Posted by: lilracerboi Posted at: 2016-09-03T01:52:41.132Z Reads: 95

```
Once I got the Space Cell in recently, I lost the luxury of an underglow using LED strips. 

Previously, I had lipos powering the motor and an external 12v DC power bank powering the lights. 

Since the Space Cell has limited room, there should be a way to power the light through the Space Cell, right?

I was thinking of using a buck converter wired between the battery and VESC. Is this a good idea? I mean, is it safe for the rest of the electronics?
```

---
## \#2 Posted by: Michaelinvegas Posted at: 2016-09-03T04:36:56.357Z Reads: 83

```
Your welcome 

https://www.ebay.com/itm/281848477612
```

---
## \#3 Posted by: lilracerboi Posted at: 2016-09-03T05:48:37.770Z Reads: 78

```
Hey, thanks a lot.

So I guess a buck converter is the answer.
```

---
## \#4 Posted by: Dedbny Posted at: 2016-09-03T06:36:42.443Z Reads: 73

```
How does that get wired up to battery? Wiring diagrams?
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2016-09-03T06:42:07.862Z Reads: 73

```
@Dedbny got a napkin I can draw on ? Lol
```

---
## \#6 Posted by: sl33py Posted at: 2016-09-03T06:50:17.891Z Reads: 69

```
@Dedbny - it has two wires in - which say voltage range.  and two wires out @ 12v 3a:
[img]http://i.ebayimg.com/images/g/0OIAAOSwo0JWOv5k/s-l1600.jpg[/img]

Doesn't get much simpler.  You'll need to power it from the power plug of the SPACE cell.  Inline or splice or whatever to tap into the power.

That make more sense?
```

---
## \#7 Posted by: Dedbny Posted at: 2016-09-03T06:52:36.837Z Reads: 68

```
So ill get 12vs out? Yeah then it is. Lots of 12v accessories.
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-09-03T07:50:20.569Z Reads: 66

```
Yeah what @sl33py said... I'm toiling on  board at the moment lol
```

---
## \#9 Posted by: sl33py Posted at: 2016-09-03T07:53:09.603Z Reads: 65

```
Yup!  12v up to 3A (realize you likely will need some airflow or it'll get hot at max amps).  But a full roll of 5050 SMD LEDs only used 1.8A when i tested, so not likely an issue unless you are riding around like @Michaelinvegas...  ;)   

I need to get one of these for eventual LED's that @Michaelinvegas showed me (the independently addressable ones) .
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2016-09-03T07:54:20.876Z Reads: 66

```
Yeah I'm delayed all over the place .... I'll get around to it soon ... I hope
```

---
## \#11 Posted by: lilracerboi Posted at: 2016-09-03T19:35:39.786Z Reads: 46

```
What are you going to do with the addressable LEDs?

I have some left over rolls of those and thought about what could be done.
```

---
