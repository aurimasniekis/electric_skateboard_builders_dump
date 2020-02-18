# Vesc question - USB to power 5v fans

### Replies: 11 Views: 408

## \#1 Posted by: Jaeson Posted at: 2018-12-02T21:42:13.606Z Reads: 119

```
@Kug3lis or @JohnnyMeduse  I thought you’d be the guys to ask. So I have a 5v usb powered fan, if I plugged the usb into one of my vescs with an adapter to mini usb, would that cause any problems? Would it work?  I have the TB vescs  and an HM-10 BT module plugged into my master. Thanks for the help! 

![image|477x500](upload://mqpWho4wTgy4eZDBrDKWku4X1i0.jpeg)
```

---
## \#2 Posted by: bigben Posted at: 2018-12-02T22:12:02.307Z Reads: 106

```
Trying to make a hoverboard?:grin:
```

---
## \#3 Posted by: Jaeson Posted at: 2018-12-02T22:13:55.658Z Reads: 105

```
Shhh I was trying to keep my plans classified.
```

---
## \#4 Posted by: Mich21050 Posted at: 2018-12-02T23:02:11.180Z Reads: 98

```
As far as I know the vesc usb port is only for input... you would need to get the 5v power from the uart power.... but you are only going to get I think 1a out of it safely :smile:
```

---
## \#5 Posted by: Blasto Posted at: 2018-12-02T23:53:33.953Z Reads: 92

```
I dont know the current conssumption of those fans, they must be under 500mA.

The resistor on your vesc supplying the 5V on the usb is most likely not populated, so it wont work
```

---
## \#6 Posted by: Jaeson Posted at: 2018-12-09T20:39:25.795Z Reads: 71

```
@Mich21050 @Blasto  So I found out that each fan pulls ~200mA 

Do you think I could remove the usb connection on the fans and wire the fans to a jst connector and plug into my slave vesc uart port? I already have a Bluetooth plugged into the master.
```

---
## \#7 Posted by: Mich21050 Posted at: 2018-12-09T20:46:26.214Z Reads: 71

```
It should be good in my oppnion. :slight_smile:
But the safest option would be @Andy87 's solutions. :slight_smile:
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-09T20:48:20.730Z Reads: 70

```
Most save way is to get a step down converter.
Connect it to your main power leads and than connect the fans to the 5V output of your step down converter.
If you have a Flipsky vesc6 they also have a 5V 1 or 2amp output. The unity should have that too.
```

---
## \#9 Posted by: Jaeson Posted at: 2018-12-09T21:00:24.987Z Reads: 63

```
Ok cool, that’s what I’ll do then. Thank you guys for the advice. 🤘🏼🤠🤙🏼
```

---
## \#10 Posted by: monsterbuilder Posted at: 2018-12-09T23:11:31.221Z Reads: 52

```
If for some reason you cannot get those to work, I'm using these in my enclosure: [link here](https://www.amazon.com/MakerFocus-Raspberry-Brushless-Connector-Separating/dp/B072FW3DDQ/ref=pd_sbs_147_1?_encoding=UTF8&pd_rd_i=B072FW3DDQ&pd_rd_r=B7D4PQW3Q9MZC7QZ895Z&pd_rd_w=u9rbG&pd_rd_wg=3kJqC&psc=1&refRID=B7D4PQW3Q9MZC7QZ895Z)

These fans can be powered off your receiver pins since most receivers output at 5V.
```

---
## \#11 Posted by: Jaeson Posted at: 2019-03-02T00:16:42.359Z Reads: 38

```
Hey guys sorry it took so long to update this thread, and not sure anyone cares, but... I went ahead and and spliced the two fans together and then soldered the wires to a 2 pin jst connector. Then I plugged it into the 3.3v and ground pins of my slave vesc’s Uart port and ⚡️⚡️ It works! 

So the answer to my original question is YES, you can power fans directly from your vesc.
```

---
