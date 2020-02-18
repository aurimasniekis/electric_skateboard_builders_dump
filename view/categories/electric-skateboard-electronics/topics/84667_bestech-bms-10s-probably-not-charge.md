# Bestech BMS 10s probably not charge

### Replies: 6 Views: 162

## \#1 Posted by: 00taffe Posted at: 2019-02-19T11:41:00.122Z Reads: 47

```
Hi guys. 
I have this Bestech BMS http://www.litechpower.com/product-detail/HCX-D596LI10S80A-04.html

The problem is that if I try to charge the batteries with a 42v 2A power supply, the circuit turned on and the VESC turns on. 

The tension at the charging port becomes 22.8v (the total of the batteries), but the power supply has 42v. 

My setup has 2 batteries (3S1P) in series. 
The charging port is attached to C- (on the BMS) and B+.

If I power on the circuit with a switch attached to the BMS, everything goes ok. 

In your opinion, what is the problem? The connection to the balance port or something else? 

Thank you very much 🙏🏻
```

---
## \#2 Posted by: Andy87 Posted at: 2019-02-19T12:10:49.276Z Reads: 41

```
the e switch needs to be turned on while charging.
if no the bms is not working
```

---
## \#3 Posted by: Andy87 Posted at: 2019-02-19T12:12:44.967Z Reads: 37

```
[quote="00taffe, post:1, topic:84667"]
charge the batteries with a 42v 2A power supply
[/quote]

[quote="00taffe, post:1, topic:84667"]
has 2 batteries (3S1P) in series
[/quote]

wo wo wo... you charge your 6s pack with a 10s charger?
```

---
## \#4 Posted by: 00taffe Posted at: 2019-02-19T12:25:58.707Z Reads: 31

```
Yes. The initial setup was of 9s but the old (very crappy) BMS broke one battery

Now I have only 2 batteries and this new BMS. The power supply is the same. 

Are there some problems with this setup? 

The e switch was tuned on but the situation is the same 
Thank you
```

---
## \#5 Posted by: Andy87 Posted at: 2019-02-19T12:29:47.427Z Reads: 31

```
your bms is no voltage regulator.
if you have a 6s battery you need to charge the battery with a 6s charger.
if you have a 10s battery you need to charge the battery with a 10s charger.
you can´t mix that up even with bms.
```

---
## \#6 Posted by: DerelictRobot Posted at: 2019-02-19T12:43:51.865Z Reads: 30

```
Correct. 

Be very, very careful. Not understanding li-ion batteries & chargers is a sure fire way to burn your house down. 

Make sure you read up and fully understand this technology, the charger requirements, and safety. These are very dangerous if you don't take the time to understand and respect the tech.

You need a matched voltage CC/CV *power supply*. They are called chargers in common vernacular but should not be confused with lipo/liion chargers which are not CC/CV
```

---
