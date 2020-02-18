# New VESC user questions

### Replies: 8 Views: 501

## \#1 Posted by: Slinge Posted at: 2017-04-27T21:48:21.094Z Reads: 79

```
So I got my vesc after riding on a car esc for over 2 years. I really get the hype now and would have bought it in the first place if I knew the difference then.

However I need some help to set it up properly. Only tried it in foc and its so good! However, when I have the board upside down the motor often wont turn. And when on the ground I need to pushstart a bit to get it going. Can I change any settings making it respond better?

Also, my biggest problem is the breaks. Only tried it for short rides.  Last night when I got it, breaks where working fine, battery was semi loaded. This morning when I got it fully loaded my breaks wouldnt take more than a second at first. It got better the more I discharged the battery but I feel that I lack in thrust with the breaks now. I understand this is to protect the battery from overcharging but is there anyway to work around it without charging the battery less than 4.35v? I run HV lipos.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-27T22:23:48.179Z Reads: 74

```
[quote="Slinge, post:1, topic:21925"]
I really get the hype now and would have bought it in the first place if I knew the difference then.
[/quote]

My thoughts exactly when I upgraded from car ESC's to Vesc's

About your brake issues, can you take a screen shot from your bldc tool first page so we can see your current and voltage settings.
```

---
## \#3 Posted by: Slinge Posted at: 2017-04-27T23:44:29.770Z Reads: 70

```
<img src="/uploads/db1493/original/3X/2/b/2b412cbb942317fe3235708f79f44b0717588ed6.jpg" width="666" height="500">
```

---
## \#4 Posted by: Blasto Posted at: 2017-04-28T01:06:02.653Z Reads: 58

```
Lower your batt max to 30A,  batt min -15

Max input voltage 57V (this is what is creating your brake issue)
```

---
## \#5 Posted by: Slinge Posted at: 2017-04-28T13:46:31.958Z Reads: 45

```
Did like you said but breaks are still cutting of.. I will see if its the same problem in bldc mode when I get back from work.
```

---
## \#6 Posted by: flywithgriff Posted at: 2017-04-28T14:24:45.261Z Reads: 44

```
Im curious as well with what adjustment makes brakes stronger! Im a bigger guy and my brakes work but a bit stronger would be great!
```

---
## \#7 Posted by: Blasto Posted at: 2017-04-28T14:29:48.618Z Reads: 40

```
[quote="flywithgriff, post:6, topic:21925, full:true"]
Im curious as well with what adjustment makes brakes stronger! Im a bigger guy and my brakes work but a bit stronger would be great!
[/quote]

Batt min is the brakes, they should be in the range of -10A to -20A

@Slinge post your motor settings again
```

---
## \#8 Posted by: Slinge Posted at: 2017-04-28T15:09:41.434Z Reads: 34

```
I thought motor min was the break strength and battery min was how much current charges the battery when breaking. Can you explain the difference? Also bat max and absolute max.

Will post settings after work in 5h.
```

---
