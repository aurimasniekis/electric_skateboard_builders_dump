# BMS wireing charge/discharge

### Replies: 10 Views: 609

## \#1 Posted by: Paalmb Posted at: 2018-04-02T09:07:56.105Z Reads: 114

```
Hi there. 
Hope you folks Can help me. 
I have Got ny hands on a bms and Would only use it to charge, not discharge. My bms does NOT have a P-.. is that Strange?
Can i do it This Way?![image|393x500](upload://5OGXUufYotnJ3rXESpdyqWsUtjn.jpeg)
```

---
## \#2 Posted by: RyuX Posted at: 2018-04-02T09:11:33.173Z Reads: 108

```
Just connect the Battery - to the VESC Directly instead going through the BMS. This will discharge directly.
the C- will only connect to the Charger. But your Regen charging will then also bypass the BMS.

I would stay safe and keep the BMS connected. Is 45A not enough for your setup ?
```

---
## \#3 Posted by: Paalmb Posted at: 2018-04-02T09:29:24.611Z Reads: 105

```
Thanx for speedy reply!
I have 10s2p Li-on 18650 batterypack. I use a vesc. 
I have some concerns about the 45A when regenerativ-Breaking. That is why i was thinking about leave the bms out when discharge, and only use it for charging. 
Think it would work??
```

---
## \#4 Posted by: rich Posted at: 2018-04-02T11:35:27.307Z Reads: 87

```
[quote="Paalmb, post:1, topic:50939"]
My bms does NOT have a P-… is that Strange?
[/quote]


No, there are different kinds of BMS, 
1. charge and discharge different port (C- = charge, P- = discharge)
2. charge and discharge same port (in your case C- = charge and discharge)

Do you have specs for the BMS, or what's the dimensions?
Maybe you can use it for discharge, too.

[quote="Paalmb, post:3, topic:50939"]
I have some concerns about the 45A when regenerativ-Breaking
[/quote]

No reason to worry
```

---
## \#5 Posted by: Paalmb Posted at: 2018-04-02T12:22:07.559Z Reads: 74

```
Here is the bms that i have. 
![image|230x500](upload://fihopcSBvrnERu3KMRGn8HqkG6g.png)
```

---
## \#6 Posted by: rich Posted at: 2018-04-02T13:34:01.981Z Reads: 58

```
Looks good, I would use it for discharge, too.
It would shut off at 130A (+-10A) which is more than you will ever discharge, especially with 2p. But you limit that in the settings anyway. Also you have to limit the batt regen to 4-5A ech vesc because of 2p. No way you will ever reach 45A.

Connect Battery (-) to BMS B-
Connect Battery (+) to charge port (+) and use it for positive discharge
Connect BMS C-  to charge port (-) and use it for negative discharge
```

---
## \#7 Posted by: Paalmb Posted at: 2018-04-02T15:39:23.869Z Reads: 56

```
Think you so much!!
```

---
## \#8 Posted by: Paalmb Posted at: 2018-04-03T17:50:49.926Z Reads: 48

```
It seems to be Working fine! Thanks again!
Just a quick question...: 
I have a 12v charger... Can i use it, or will it fry?
```

---
## \#9 Posted by: rich Posted at: 2018-04-03T18:03:16.268Z Reads: 48

```
Do you mean 12V input or output voltage?
For 10s you need a 42V Li-ion charger.
```

---
## \#10 Posted by: Paalmb Posted at: 2018-04-03T19:00:51.081Z Reads: 45

```
Og sorry. Of course output. 
I order one strait away
Thank again
```

---
