# Latching switch: SPDT (On-On) vs SPDT (1NO1NC)

### Replies: 10 Views: 1056

## \#1 Posted by: RiGo Posted at: 2017-08-08T06:24:50.623Z Reads: 71

```
Just wondering if there's a difference between these switch configurations?

Wanna get me one of these (to use with a Vedder anti-spark):

http://au.rs-online.com/web/c/switches/push-button-switches-accessories/push-button-switches/?rpp=100&applied-dimensions=4294615441,4293690593

But not sure if On-On is the same as 1NO1NC. It should be, right?

Thanks!!!
```

---
## \#2 Posted by: krloz Posted at: 2017-08-08T09:03:32.004Z Reads: 60

```
I think the on on means that both positions of the switch are wired and usable. And the 1no1nc means that one of the circuits is opened and the other one closed in one of the switch positions and swap in the other position. So I think yeah they are the same.  In any case the second one could be a switch with two contacts for the no position and two other contacts for the nc position.  Ie with no comm. But even then you can wire together a contract of each side making a comm connection
```

---
## \#3 Posted by: darkkevind Posted at: 2017-08-08T10:18:56.539Z Reads: 58

```
Those switches won't work because there are basically two positions with a common ground.

ON will be latched in an ON position for one circuit, so constantly on, then if you press that button again, you're turning on another circuit but only momentarily, and in doing that it breaks the original ON circuit.

You need ON-OFF / OFF-ON latching and not momentary.
```

---
## \#4 Posted by: MontPierre Posted at: 2017-08-08T10:28:58.342Z Reads: 53

```
You can also look for " SPDT switch" - latching, 12V - those will work, I have one myself with LED from eBay. 


https://www.ebay.co.uk/itm/142394830989 

Great build quality but a little long - check measurements to see it if fits your enclosure.

To have LED working you will need resistor.

Here is wiring diagram + resistor values depending on your battery voltage.

<img src="/uploads/db1493/original/3X/7/b/7b2c7f14f6f2cedff6d4ec04d7c0fa32ea0617dc.PNG" width="690" height="238"><img src="/uploads/db1493/original/3X/a/4/a4b539ee9be2a119a4e4dc80a60ce4bbe943dd56.PNG" width="665" height="500">

Resistor can be found on RS online ;)
```

---
## \#5 Posted by: darkkevind Posted at: 2017-08-08T10:33:45.455Z Reads: 45

```
[quote="MontPierre, post:4, topic:30037"]
To have LED working you will need resistor.
[/quote]

A voltage regulator would be better than a resistor...
```

---
## \#6 Posted by: MontPierre Posted at: 2017-08-08T10:40:05.215Z Reads: 44

```
True but it will take more space in enclosure . 12V rated button works fine with 41V so far and I have seen a lot of guys here with the same button.
```

---
## \#7 Posted by: darkkevind Posted at: 2017-08-08T10:58:40.448Z Reads: 41

```
Not much room at all, just a couple of CM(cubed).

I'd worry about the resistor burning up and causing excess heat bringing the power down from 30v+ to 1.5v for the LED...
```

---
## \#8 Posted by: RiGo Posted at: 2017-08-09T00:13:11.012Z Reads: 34

```
These are all latching switches with a common and two separate circuits that are closed depending on the position of the switch (button up, or button latched down).

So if one is closed, then the other one's open, and vice versa.

So this should be the same as NO NC. Hence my question.
```

---
## \#9 Posted by: RiGo Posted at: 2017-08-09T00:14:15.953Z Reads: 33

```
These are latching SPDT witches. They're labeled as on-on, instead of NONC but as I see it they should be the same thing.

Just wanted to confirm, hence the post.
```

---
## \#10 Posted by: MontPierre Posted at: 2017-08-09T00:25:04.580Z Reads: 31

```
They work with my antispark perfectly ;)
```

---
