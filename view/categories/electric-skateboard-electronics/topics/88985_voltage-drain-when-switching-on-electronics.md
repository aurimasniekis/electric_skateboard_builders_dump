# Voltage drain when switching on Electronics

### Replies: 12 Views: 146

## \#1 Posted by: Z4MSupreme Posted at: 2019-04-01T14:03:27.658Z Reads: 63

```
Hi guys,

I've just gone to plug all my electronics together ready to fit onto my board and when I turn it on everything lights up and then fades away in a couple of seconds. The voltage also goes up to normal voltage and drops to about 5v in a couple of seconds

Im not sure what the problem could be as it worked when I previously tested it. Nothing smells burnt so not sure what the issue is.  

I really appreciate any help. Thanks
```

---
## \#2 Posted by: banjaxxed Posted at: 2019-04-01T14:22:33.709Z Reads: 55

```
Antispark?
```

---
## \#3 Posted by: Mich21050 Posted at: 2019-04-01T14:25:51.689Z Reads: 50

```
We need a bit more information about your setup. Vesc, battery, antispark and so on.
```

---
## \#4 Posted by: Z4MSupreme Posted at: 2019-04-01T14:32:52.033Z Reads: 48

```
I am using a 10s3p pack with 30q batteries and a 10s bestech bms with an led e switch. With a voltmeter, the voltage will go to 36 volts and then drop back down. And the led on the switch fades off.
```

---
## \#5 Posted by: Z4MSupreme Posted at: 2019-04-01T14:33:06.163Z Reads: 47

```
I am using the eswitch on a Bestech 10s bms
```

---
## \#6 Posted by: Z4MSupreme Posted at: 2019-04-01T14:35:31.851Z Reads: 44

```
Also, when I plug it into charge the voltmeter goes up 1 percent about every 10 seconds. And it's only a 2A charger
```

---
## \#7 Posted by: olestra Posted at: 2019-04-01T15:07:22.809Z Reads: 40

```
test the voltage before the BMS when this happens -- if the volts before BMS don't drop -- the BMS must be defective.
if the volts before BMS still drop, then you must have bad cells.
```

---
## \#8 Posted by: Z4MSupreme Posted at: 2019-04-01T15:31:54.150Z Reads: 34

```
I have just checked and one of the cells was at 3.0v. I have put it on charge to hopefully balance them, and then the BMS will stay on. Thanks for your help :)
```

---
## \#9 Posted by: olestra Posted at: 2019-04-01T15:40:11.389Z Reads: 31

```
that would do it! good luck
```

---
## \#10 Posted by: Z4MSupreme Posted at: 2019-04-01T16:05:18.950Z Reads: 28

```
Thank you. I just took it off charge and it stayed on so all fixed :smile:
```

---
## \#11 Posted by: DEEIF Posted at: 2019-04-01T16:07:27.671Z Reads: 28

```
@mmaner @mmaner @mmaner
```

---
## \#12 Posted by: mmaner Posted at: 2019-04-01T18:23:17.083Z Reads: 17

```

```

---
