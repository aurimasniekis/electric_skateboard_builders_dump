# Does a BMS shut off power?

### Replies: 6 Views: 291

## \#1 Posted by: jason182 Posted at: 2018-08-03T11:51:14.296Z Reads: 70

```
Does a BMS shut power off when the battery is discharged or does it just monitor the rate at which a battery discharges? I’m a little confused on having a BMS then setting voltage warning and cut off levels on the vesc. Any clarification from a person with knowledgeable advice on the matter would be much appreciated.
```

---
## \#2 Posted by: Andy87 Posted at: 2018-08-03T11:55:59.285Z Reads: 70

```
Your bms will shit down your battery.
If you set your vesc cut off higher than your bms cut off than the vesc will shut off
```

---
## \#3 Posted by: Erniechan Posted at: 2018-08-03T12:09:34.571Z Reads: 66

```
Yes the bms will protect overdischarge issues.
The lvc will cut power somewhere between 3.0v and 2.5v for li ion depending on the bms(different voltages for other chemistry cells) Also the hvc will avoid overcharge and cut load at 4.2 volts(different again for lifepo4 for example).
```

---
## \#4 Posted by: deucesdown Posted at: 2018-08-03T13:00:41.355Z Reads: 55

```
[quote="Andy87, post:2, topic:63702"]
Your bms will shit down your battery.
[/quote]

That's a shit bms
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-03T13:15:47.658Z Reads: 49

```
Just important the bms safe the battery from over discharge☝️ Doesn’t matter how it’s working technically...if shut off or to shit off...the result matters😌😌😌☝️😌
```

---
## \#6 Posted by: dareno Posted at: 2018-08-04T01:12:09.640Z Reads: 29

```
I'm still giggling
```

---
