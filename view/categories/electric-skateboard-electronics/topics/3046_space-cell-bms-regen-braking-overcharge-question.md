# SPACE Cell BMS regen-braking overcharge question

### Replies: 12 Views: 1662

## \#1 Posted by: AlMcCal Posted at: 2016-05-09T23:13:58.587Z Reads: 172

```
Hey everyone I'm new to the e-skate world, first off thanks for all the info I've been able to find here. I'm building, my first board and there is a question I haven't been able to figure out regarding regenerative braking with a vesc and space cell. If you brake with a full charge in the space cell will it over charge the 18650 cells?  My question arose when doing research on BMS's and I noticed that most have a separate discharge lead than charge lead which means the mosfets only have a low voltage cutoff on the discharge and high voltage cutoff on the charge so they won't shut off of when the regen is over charging the battery through the discharge lead. I was wondering if the space cell works around this problem with any of the following solutions:

--Regen current is redirected through the charge lead with diodes 
--BMS is designed with high voltage cutoff on the discharge lead
--don't break when your battery is above a certain percentage

Thanks for your help!
```

---
## \#2 Posted by: willpark16 Posted at: 2016-05-09T23:15:33.876Z Reads: 168

```
well most likely you wont brake without first using a bit of power to get going also no it wont because u have a 40a fuse to prevent this from happening.
```

---
## \#3 Posted by: willpark16 Posted at: 2016-05-09T23:16:24.685Z Reads: 169

```
Also I would like to thank you for coming to this forum with a bit of knowledge already and not empty handed
```

---
## \#4 Posted by: AlMcCal Posted at: 2016-05-09T23:18:56.136Z Reads: 158

```
Thanks Will, I guess I might just be over thinking the issue
```

---
## \#5 Posted by: willpark16 Posted at: 2016-05-09T23:20:56.472Z Reads: 154

```
haha no problem and everyone does on their first build. Have u decided on the rest of your parts yet or are u gonna do all enertion brand?
```

---
## \#6 Posted by: AlMcCal Posted at: 2016-05-09T23:29:23.053Z Reads: 149

```
So I was originally thinking of going with LifePO4 38120s cells because of their stability and long life but the shipping from china was way too expensive so I will probably go with LiNiCoAlO2 18650 He2 cells which are on amazon and do a setup like the space cell with a BMS from Battery Supports. I've ordered a vesc from enertion and an SK3 from hobby king. I'll cnc my own motor mount.
```

---
## \#7 Posted by: Kaly Posted at: 2016-05-10T00:35:07.518Z Reads: 138

```
Do not worry about the regen current over charging your battery unless you start by going down hill from the get go. The regen current is not that big and the current fluctuates so the cell will push resist any charging that is not constant current at least in real world usage.
```

---
## \#8 Posted by: willpark16 Posted at: 2016-05-10T00:40:47.596Z Reads: 140

```
dont order from amazon go to li ion wholesale on google way better prices
```

---
## \#9 Posted by: WrinklyWink Posted at: 2016-05-11T09:48:12.727Z Reads: 117

```
would regenerative breaking current destroy or damage an UBEC on the same power leads? I want to add and use a separate voltage for lights without having to resort to another battery..
```

---
## \#10 Posted by: Kaly Posted at: 2016-05-11T10:31:42.224Z Reads: 114

```
No , the regen current will not damage the ubec.
```

---
## \#11 Posted by: thisrealhuman Posted at: 2016-05-11T11:48:27.664Z Reads: 107

```
[quote="Kaly, post:10, topic:3046"]
the regen current will not damage the ubec
[/quote]

Wrong, ive killed two ubecs. My situation was that the loop fell out while riding, so the power generated went only into my ubec. If you are only breaking normal and not trying to break down a monster hill im sure you will be fine, but if you pop the space cell fuse the power will still have somewhere to go.
```

---
## \#12 Posted by: Kaly Posted at: 2016-05-11T18:09:47.924Z Reads: 95

```
You answered your self. 
[quote="thisrealhuman, post:11, topic:3046"]
My situation was that the loop fell out while riding, so the power generated went only into my ubec.
[/quote]

 In normal conditions the regen current do not damage the UBEC. 

Your case is a battery system malfunction or user mistake. 

@thisrealhuman I advice you read and analyze what you write before pressing reply. I prefer to comment just on issues I really understand. Don't like to send people in the wrong direction.
```

---
