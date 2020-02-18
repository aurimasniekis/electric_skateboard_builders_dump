# Anti-spark mosfet question

### Replies: 5 Views: 412

## \#1 Posted by: jimi Posted at: 2017-12-11T09:07:53.502Z Reads: 113

```
On a Vedder-type anti-spark switch, Is there any need to electrically isolate the drain of the mosfet(s) from the heat sink since the drain is connected to vesc ground?
```

---
## \#2 Posted by: Quezacotl Posted at: 2017-12-11T10:24:07.423Z Reads: 97

```
No need to isolate as long as it doesn't touch anywhere else.
What was your concern?
```

---
## \#3 Posted by: Martinsp Posted at: 2017-12-11T18:13:06.725Z Reads: 79

```
You dont necessarily need to isolate it but I highly reccomend you to do so. The best way to achieve this is to buy a piece big enough to cover your direct fets. It conducts heat very well and at the same time does not conduct electricity. The same thing is used in FOCBOXes and other applications. You dont need to do it of course but I would simply for peace of mind and safety. You avoid burning your stuff. It is really cheap, roughly the same price of a thermal paste.
```

---
## \#4 Posted by: Martinsp Posted at: 2017-12-11T18:14:48.999Z Reads: 78

```
Not sure what dimensions you need but have a look here: http://www.ebay.com/bhp/thermal-conductive-pad
You can always order bigger piece and cut it so you should be able to find a piece big enough.
```

---
## \#5 Posted by: jimi Posted at: 2017-12-12T02:38:59.354Z Reads: 48

```
Believe it or not I'm a retired EE with experience in electrical safety but I trust people with hands-on experience more than I trust my own instincts. I want to do things right the first time.
```

---
