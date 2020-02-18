# Good 36V(10S) chargers?

### Replies: 6 Views: 1413

## \#1 Posted by: KTMinni Posted at: 2017-03-16T00:58:07.095Z Reads: 250

```
So I am trying to find the last part to my project and that is the charger, I have my 18650 batteries wired up in a 10S2P config. The only reasonable charger I could find was this 36V 1.6A one:
https://www.electricscooterparts.com/36vchargers.html

other than that I have had trouble finding a charger that won't cause my board to explode or melt.

Anyone else have a similar problem?
```

---
## \#2 Posted by: Randyc1 Posted at: 2017-03-16T01:07:46.925Z Reads: 248

```
Search 36V(42V) lithium Ion chargers.alibaba
```

---
## \#3 Posted by: Namasaki Posted at: 2017-03-16T01:53:58.856Z Reads: 240

```
4.2v is full charge on a Li-ion 18650 3.6 is the nominal voltage so what you need is a 42v charger.
There are a ton of them out there on eBay. 2a and 5a 
Just search for 42v chargers and you'll find plenty
http://www.ebay.com/itm/Universal-Charger-42V-2A-Adapter-For-Hoverboard-Smart-Balance-Scooter-Wheel-US-/332136054967?hash=item4d54da00b7:g:NhgAAOSwfVpYroIn
```

---
## \#4 Posted by: Namasaki Posted at: 2017-03-16T02:34:22.945Z Reads: 224

```
Did you wire in a BMS on your battery ?
```

---
## \#5 Posted by: KTMinni Posted at: 2017-03-16T12:58:07.674Z Reads: 206

```
Yes, I did wire in a 50A BMS so I might need to bypass for discharge
```

---
## \#6 Posted by: Namasaki Posted at: 2017-03-16T13:13:35.823Z Reads: 196

```
You should be ok to discharge through a 50a BMS. 
Just set your Vesc current max accordingly in bldc tool
```

---
