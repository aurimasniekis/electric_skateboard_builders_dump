# 12s has no negative lead on balance connector?

### Replies: 4 Views: 273

## \#1 Posted by: Sigorr Posted at: 2018-06-12T02:58:11.899Z Reads: 56

```
Hello I'm trying to put together an e-longboard and i cant find the answer to this on google. So I have made a battery diagram and planning to use a bms here is the 12s4p battery:![IMG_20180531_185700524|666x500](upload://1ghCKctWwRR3OKAJyY5fdTZozz0.jpg)

The thing I ran in to is that my diagram has 13wires for the Ballance connector but all of the bms have 12 pin for 12s battery. If remove the wire that is labeled 0 would it still work? Can someone explain this to me? Do I not need a negative lead for the balance connector?

Also what do you guys think of this bms, I don't need a high amp rating because I'm not using the bms for discharging

https://bmsbattery.com/ebike-battery/322-12s-lifepo4-bms-battery-management-system-battery.html#/212-discharge_current-20_40a
```

---
## \#2 Posted by: i2oadsweepei2 Posted at: 2018-06-12T10:22:40.830Z Reads: 43

```
As far as I know you would delete the “0” from your diagram. That is what the diagram shows. No balance lead to the negative. B- to the battery negative and B1 starts at the first series connection.

![image|666x500](upload://2YRvK16ZYPEx5WenBtr6XiY573m.jpg)
```

---
## \#3 Posted by: JonathanLau1983 Posted at: 2018-06-12T11:12:43.123Z Reads: 35

```
I think it's because the BMS is expecting the negative to be used for discharge and so it will be using the main -B on the BMS, no need for balance connector.
```

---
## \#4 Posted by: rich Posted at: 2018-06-12T14:29:59.518Z Reads: 27

```
[quote="Sigorr, post:1, topic:58613"]
all of the bms have 12 pin for 12s battery
[/quote]


There are different BMS existing, some have 12, some have 13 pins for 12s. This depends on the BMS.

Do you build a Li-ion or a LiFePO4 battery because if it's Li-ion then the BMS is the wrong one.
```

---
