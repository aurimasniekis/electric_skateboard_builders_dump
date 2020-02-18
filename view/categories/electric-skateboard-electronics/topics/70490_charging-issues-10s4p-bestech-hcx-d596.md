# Charging issues (10s4p, Bestech hcx-d596)

### Replies: 3 Views: 191

## \#1 Posted by: hungoverpilot Posted at: 2018-10-08T00:08:20.322Z Reads: 46

```
Hey all,

I just finished my battery build.  Got the motors all hooked up and working properly.  Plugged it into charge for an hour and it hasnt moved voltage at all.  I made sure to have the BMS eswitch turned on while charging.  But there has been some strange behaviour while the charger is plugged in.  If i plug the charger into the charging port, but leave the charger unplugged from the wall, the light on the charging brick turns on (See pic below, charging port is in background)

![20181007_165445|375x500](upload://oGPj4MtM3uleZPeRB6FigAMQmo0.jpeg) 

Also, when i plug the charger into the board, and connect it to the wall, (but have not turned on the bms eswitch yet) the vescs seem like they are power cycling.  I thought they shouldnt get any power at all unless the eswitch is on?

Here is the charger im using:

![20181007_164513|375x500](upload://dkyM0EbQAKVZJvIeV7zCYETIqcT.jpeg) 

Battery is 10s4p Samsung 30Q, all balance leads to BMS are measuring correct voltage.  Any ideas on whats wrong?? Thanks.
```

---
## \#2 Posted by: chickengun Posted at: 2018-10-08T00:29:11.667Z Reads: 38

```
your charger has a DC ouput voltage of 36V, but you need 42V.
```

---
## \#3 Posted by: mynamesmatt Posted at: 2018-10-08T06:28:19.246Z Reads: 32

```
[quote="chickengun, post:2, topic:70490"]
you need 42V
[/quote]

^ thats your answer. Nominal (average) voltage of your pack is 36V but the fully charged voltage is 42V so thats what ya need. They're pretty cheap on eBay
```

---
