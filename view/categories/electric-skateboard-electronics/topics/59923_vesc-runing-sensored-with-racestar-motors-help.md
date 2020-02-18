# VESC runing sensored with racestar motors - HELP

### Replies: 7 Views: 246

## \#1 Posted by: shaohad Posted at: 2018-06-24T16:59:53.635Z Reads: 68

```
Hello. eveyone.
i have the racestar motors and vescs id like to run the motors in sensored mode.
when try to do the decation one motor did it corectly and show the sensors table and and the other motor give hall sensors detection failed.
any easy idea to solve that? 
i have maytec vescs
regards
```

---
## \#2 Posted by: SeanHacker Posted at: 2018-06-24T17:02:43.124Z Reads: 64

```
What kind of fail do you mean? Was it stuttering too much? Sensor error? 

If it's stuttering too much then up the duty cycle to .15 and try again.
```

---
## \#3 Posted by: shaohad Posted at: 2018-06-24T17:20:14.420Z Reads: 56

```
the hall sensors detaction is failed .
```

---
## \#4 Posted by: Sender Posted at: 2018-06-24T17:30:05.322Z Reads: 52

```
Put up some screen shots of your settings.


Are you running FOC? Which firmware?

You could try raising the amps to 10 for detetection.
```

---
## \#5 Posted by: rich Posted at: 2018-06-24T21:33:32.470Z Reads: 45

```
Take the "bad" motor and do detection on the vesc where you get the proper hall sensor table then you know if its the motor or the vesc. I had the same problem with 2 Maytech vescs and one had a cold solder joint on one pin of the hall sensor port on PCB.
```

---
## \#6 Posted by: briman05 Posted at: 2018-06-25T04:03:18.241Z Reads: 35

```
Same thing happened to me. I put on acks firmware and ran it in fox and it detected the sensors first time.
```

---
## \#7 Posted by: shaohad Posted at: 2018-06-25T05:43:01.098Z Reads: 30

```
i am runing in BLDC do not like to go to FOC since i do not have enough knowledge and do not have the time to learn.
just wanna ride.
now idea what "rab in fox" meaning is.
```

---
