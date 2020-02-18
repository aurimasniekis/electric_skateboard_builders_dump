# VESC and motor issues?

### Replies: 15 Views: 605

## \#1 Posted by: esk8guy Posted at: 2018-01-30T06:46:06.840Z Reads: 65

```
i am building a dual motor board and both vescs have been programmed. When i start the motors up one starts normally and the other is a bit sluggish until i push down the throttle a little further. Is this an issue with my remote settings or do i need to look into issues with the motor itself? has anyone else had this issue on a dual motor set up?
```

---
## \#2 Posted by: Colson003 Posted at: 2018-01-30T06:49:40.870Z Reads: 64

```
Sensored or sensorless?
```

---
## \#4 Posted by: esk8guy Posted at: 2018-01-30T06:52:33.076Z Reads: 60

```
sensorless 280kv motor and it is running on 6s 12000mah pack
```

---
## \#5 Posted by: Colson003 Posted at: 2018-01-30T06:55:21.217Z Reads: 55

```
I have the same thing happen to me sometimes too. Also on 6s sensorless. see how it behaves with you on it from a standstill.

Foc or bldc?
```

---
## \#6 Posted by: esk8guy Posted at: 2018-01-30T06:56:55.571Z Reads: 51

```
i actually tested it a bit earlier and it was able to start up from a standstill with me on it which was pretty good considering the last board i made did not. Even though it starts up im skeptical as to if it is reaching max speed if its not calibrated right
```

---
## \#7 Posted by: esk8guy Posted at: 2018-01-30T06:57:30.121Z Reads: 48

```
bldc. i heard foc has issues with breaking.
```

---
## \#8 Posted by: Colson003 Posted at: 2018-01-30T06:58:37.811Z Reads: 45

```
Yeah I doubt there's any issue. What FW are you on? And what vesc are you using?
```

---
## \#9 Posted by: esk8guy Posted at: 2018-01-30T06:59:57.294Z Reads: 46

```
sorry im not sure what FW means. i am using the VESC 4.12
```

---
## \#10 Posted by: Colson003 Posted at: 2018-01-30T07:00:55.407Z Reads: 44

```
What firmware, 2.18? 3.30? 2.54? I mean where did you get the vesc from?
```

---
## \#11 Posted by: esk8guy Posted at: 2018-01-30T07:03:31.446Z Reads: 43

```
I bought them from eBay from a seller named softempower
```

---
## \#12 Posted by: esk8guy Posted at: 2018-01-30T07:04:34.010Z Reads: 40

```
forgot to reply with @ sorry
```

---
## \#13 Posted by: Colson003 Posted at: 2018-01-30T07:07:16.646Z Reads: 40

```
Hmm looks to me like it's a maytech. Not 100% though. Stick with bldc unless you wanna risk it.
```

---
## \#14 Posted by: esk8guy Posted at: 2018-01-30T07:08:03.700Z Reads: 42

```
what issues would i have with foc? i havent done much research on it but from what ive heard it was just an issue with stopping. is there anything else i need to be looking out for?
```

---
## \#15 Posted by: Colson003 Posted at: 2018-01-30T07:10:56.056Z Reads: 44

```
I do run foc and I haven't had any issues braking, some of the older firmware versions could have a boost effect when approaching top speed. I had that when running foc on 2.18fw. 

Since updating to 3.34fw with the vesc-tool that has disappeared. 

Just be sure to follow the setup process correctly, which on the vesc-tool is dead simple.
```

---
## \#16 Posted by: JohnyVes Posted at: 2018-01-31T17:41:35.409Z Reads: 30

```
Hey, I´ve problem with 2 FOCBOX´s. During the ride very often motors turning off (for 1 sec or 2 sec.) and again ride normall. 2 months ago, I set the FOCBOX too and all is OK. I use same steps. Motors turning off when I using single or dual motors (not fault in CAN-BUS) all others parts are OK. Maybe I have 2 FOCBOX wrong 
(I dont believe it) or is some problem in settings. Have somebody same problem?
(Used: Ackmaniac bldc tool, VESC-tool (vesc-project.com), Ackmaniac vesc-tool) - for every SW must used different fw. Thanks for advices.
```

---
