# Motor detection failed

### Replies: 13 Views: 819

## \#1 Posted by: bbiniyam Posted at: 2017-07-23T02:37:59.637Z Reads: 69

```
Hi guys I am configuring my brand new enertion VESC-X with a torque board 6354 260 kv motor. I have a 6s setup and i am trying to do motor detection. When I click start detection, my motor spins really fast then it stops Then I get "Bad Detection Result Recieved"
```

---
## \#2 Posted by: flywithgriff Posted at: 2017-07-23T02:47:10.195Z Reads: 68

```
Post photos of your settings.
```

---
## \#3 Posted by: bbiniyam Posted at: 2017-07-23T03:02:06.456Z Reads: 68

```
<img src="/uploads/db1493/original/3X/1/4/14ffd2c41bc07f51cd2d9e0f30f2ac74c5e37f08.png" width="689" height="459"><img src="/uploads/db1493/original/3X/8/d/8d55bef7ef055ecd375da12eb8bc4475019a2cd3.png" width="689" height="459">
```

---
## \#4 Posted by: bbiniyam Posted at: 2017-07-23T03:03:48.078Z Reads: 59

```
the motor spins but when you put some wight or put the long board down and hit the throttle it wont move.
```

---
## \#5 Posted by: Blasto Posted at: 2017-07-23T03:06:36.612Z Reads: 61

```
Check this thread... make sure todo a motor detection or you will damage your hardware

http://www.electric-skateboard.builders/t/solved-please-help-motor-is-having-trouble-moving-the-weight-of-the-board-without-me-standing-on-it/28183?u=blasto
```

---
## \#6 Posted by: bbiniyam Posted at: 2017-07-23T03:19:43.921Z Reads: 55

```
still getting bad detection result received.
```

---
## \#7 Posted by: rpn314 Posted at: 2017-07-23T03:24:35.829Z Reads: 55

```
If you ever get a bad detection, you should not be putting any weight on it at all. That needs to be fixed before it will every work properly.

Have you read thru the entire thread that @Blasto linked to?
```

---
## \#8 Posted by: bbiniyam Posted at: 2017-07-23T03:27:37.256Z Reads: 54

```
got it now its working fine. tnx for helping out
```

---
## \#9 Posted by: FMS Posted at: 2017-07-23T03:28:28.602Z Reads: 54

```
Where are you guys getting the BLDC tool? Everywhere I've looked so far has broken links.
```

---
## \#10 Posted by: rpn314 Posted at: 2017-07-23T03:31:02.311Z Reads: 53

```
[quote="FMS, post:9, topic:28338, full:true"]
Where are you guys getting the BLDC tool? Everywhere I've looked so far has broken links.
[/quote]


That's a bit of a topic hijack, but here's your answer.

http://www.electric-skateboard.builders/t/where-to-get-old-version-of-bldc-tool/27328?u=rpn314
```

---
## \#11 Posted by: bbiniyam Posted at: 2017-07-23T14:54:17.751Z Reads: 42

```
he you guys can download bldc tool here https://drive.google.com/file/d/0B0o_3IlBcNTlYVNvM2djaUFZZkE/view
```

---
## \#12 Posted by: darkkevind Posted at: 2017-07-23T15:06:54.392Z Reads: 41

```
If you're getting bad detection, up the amps on the test until it detects properly, 8-10A should give you a good result.
```

---
## \#13 Posted by: JohnnyMeduse Posted at: 2017-07-23T15:14:08.001Z Reads: 39

```
it might be the Battery cutoff (In the Motor Configuration Tab), put the cutoff start at around 19,20V and the cutoff end at 18V.
```

---
