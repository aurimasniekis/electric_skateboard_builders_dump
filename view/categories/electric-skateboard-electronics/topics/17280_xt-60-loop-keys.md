# Xt-60 loop keys

### Replies: 8 Views: 1148

## \#1 Posted by: ZachNYC Posted at: 2017-02-06T02:45:39.820Z Reads: 154

```
I'm using xt-60s loop keys to be able to take my batteries apart for airplanes, just wondering what I should use to complete the loop, would copper ground wire work here as well?
```

---
## \#2 Posted by: jmasta Posted at: 2017-02-06T02:56:50.121Z Reads: 152

```
XT-60 does not come in an anti-spark variant.  You would need an XT-90S, which is denoted with a green stripe... Or else you're going to get a huge spark every time you connect the loop key
```

---
## \#3 Posted by: ZachNYC Posted at: 2017-02-06T02:58:13.418Z Reads: 151

```
I have one, I'm not talking about powering the board on, I'm talking about connecting and disconnecting the batteries for airplanes like this, http://www.electric-skateboard.builders/t/first-build-loaded-vanguard-deck-1-turnigy-sk3-6374-192kv-12s3p-samsung-25r-vesc-x/14242/54?u=zachnyc
```

---
## \#4 Posted by: NewbieBoardBuilder Posted at: 2017-02-06T18:45:04.881Z Reads: 94

```
[quote="jmasta, post:2, topic:17280"]
XT-60 does not come in an anti-spark variant.  You would need an XT-90S, which is denoted with a green stripe...
[/quote]

What is the difference between xt-90 and xt-90S?
```

---
## \#5 Posted by: Smorto Posted at: 2017-02-06T18:46:39.948Z Reads: 80

```
Simple answer is that XT90-S has an anti spark future while XT90 is just a connector. They are both the same shape though.
```

---
## \#6 Posted by: NewbieBoardBuilder Posted at: 2017-02-06T18:47:33.328Z Reads: 81

```
Is there the same thing for 60s?
```

---
## \#7 Posted by: Smorto Posted at: 2017-02-06T18:47:52.864Z Reads: 77

```
Not to my knowledge no. Although, I use all XT60 connectors on my board except for 1 XT90-S as the switch/anti-spark loop.
```

---
## \#8 Posted by: jmasta Posted at: 2017-02-06T19:23:34.791Z Reads: 69

```
[quote="NewbieBoardBuilder, post:4, topic:17280, full:true"]
What is the difference between xt-90 and xt-90S?
[/quote]

XT-90S (Anti-Spark variant) has a two-stage connection on the positive terminal.  First it connects the load with a resistor wired in series; this slows the in-rush of current to the capacitors, preventing the spark.  Then once the XT90S is fully connected, it completes the circuit with no resistor

<img src="/uploads/db1493/original/3X/d/c/dc9d848696e354be9f36abe7588799409043d22b.png" width="323" height="458">
```

---
