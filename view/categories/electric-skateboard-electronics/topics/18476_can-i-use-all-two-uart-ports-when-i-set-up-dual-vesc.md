# Can i use all two UART ports when i set up dual Vesc?

### Replies: 4 Views: 632

## \#1 Posted by: Fabian287 Posted at: 2017-03-02T19:25:46.049Z Reads: 91

```
Hey there,

i want to build my 2.0 Electric skateboad. I use dual vesc. I want to contol my ArduBoardController(nunchuck) with one UART port and i want also to set up a HM-10 bluetooth module. My Vescs are connected over Can-bus. Will it work or can i just use one UART port? :slight_smile:

sry for my english im german ^^
```

---
## \#2 Posted by: Blasto Posted at: 2017-03-02T19:31:08.610Z Reads: 88

```
I would think it would work. Basically you have your hm-10 on the slave vesc, it's receiving it's commands via the can bus. Just need to activate the uart app on the slave
```

---
## \#3 Posted by: Fabian287 Posted at: 2017-03-02T21:35:34.123Z Reads: 71

```
i want to use the bluetooth module to control the metr app. so you think it will work?
```

---
## \#4 Posted by: rpn314 Posted at: 2017-03-03T01:29:00.314Z Reads: 58

```
Yes it will. Source: I do almost the same thing
```

---
