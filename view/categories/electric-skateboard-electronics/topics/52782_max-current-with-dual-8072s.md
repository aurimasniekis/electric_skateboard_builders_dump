# Max current with dual 8072S’?

### Replies: 18 Views: 722

## \#1 Posted by: chocol4te Posted at: 2018-04-19T12:50:49.290Z Reads: 145

```
Hello!

I am trying to calculate the max current I will need for a dual 8072S build. I’ve got a few different configurations and not sure which will be the most the demanding. The motor is rated for 6kW and 95A max, but I doubt dual would mean my batteries should supply 190A. What would typical draw look like with the following configurations?

Fixed:
* 12S 30Q battery
* 80kg max board and rider weight 
* 25% grade hills

Variable: 
* Single 8072S vs dual upgrade later on
* 14:66 and 18:66 gearing
* 6.5” street tyres and 125mm Gummies

Thanks! :slight_smile:
```

---
## \#2 Posted by: Cobber Posted at: 2018-04-19T12:53:40.087Z Reads: 143

```
What voltage is the motor rated for?

Amps * volts = watts
```

---
## \#3 Posted by: chocol4te Posted at: 2018-04-19T12:58:52.204Z Reads: 140

```
It’s rated for 15S, I’ll be using a 12S.
```

---
## \#4 Posted by: Cobber Posted at: 2018-04-19T14:47:21.039Z Reads: 118

```
what speed controller are you going to use?
```

---
## \#5 Posted by: chocol4te Posted at: 2018-04-19T15:07:34.040Z Reads: 111

```
ESCapes
10char
```

---
## \#6 Posted by: Exiledd_Top Posted at: 2018-04-19T15:10:27.776Z Reads: 104

```
Those trampa builds usually are big money with 8000x motors and if you got a escape and want the desired amps go Lipo route but get tattu batteries there  like the best thing that happened to 8000x motors
```

---
## \#7 Posted by: Deckoz Posted at: 2018-04-19T15:14:15.399Z Reads: 101

```
How much do you weigh is the real question....
```

---
## \#8 Posted by: chocol4te Posted at: 2018-04-19T15:20:03.210Z Reads: 95

```
I weigh 72kg, board will be ~8kg dependant in which batteries I go with
```

---
## \#10 Posted by: chocol4te Posted at: 2018-04-19T15:21:29.255Z Reads: 93

```
Thanks! I was thinking of making a Kaly style enclosure, but double height for a theoretical 12s8p pack. Will that be enough current?
```

---
## \#11 Posted by: Exiledd_Top Posted at: 2018-04-19T16:21:36.161Z Reads: 83

```
12s8p 8pX20 on 30q is 160amps I think that would be fine but that's going to cost a lot,  keep in mind that thing is going to weigh alot as well .
```

---
## \#12 Posted by: chocol4te Posted at: 2018-04-19T16:27:57.757Z Reads: 83

```
That’s what I was thinking, it would be pretty unweildy. 12s4p is 80 amps, will I ever draw that?
```

---
## \#13 Posted by: E1Allen Posted at: 2018-04-19T18:36:55.653Z Reads: 67

```
Yes. You should easily draw that if you are okay with hard acceleration.
```

---
## \#14 Posted by: chocol4te Posted at: 2018-04-19T19:41:55.160Z Reads: 59

```
Sorry, I should have been clearer, will 12s4p be enough for a dual 8072S build or do I need to go higher? I’m thinking that if I build my own enclosure, I should be able to fit a 12s5p on the Carver without doubling up.
```

---
## \#15 Posted by: E1Allen Posted at: 2018-04-19T20:12:29.194Z Reads: 53

```
If I were building it with large motors like 8072 I'd go for sure with 5p or higher.  You can limit battery amps per vesc to not exceed what your battery can put out.  Then set motor amps to 95a each.
```

---
## \#17 Posted by: Kug3lis Posted at: 2018-04-19T20:34:08.402Z Reads: 48

```
I tried today full power on my motors 90A/motor went out never even reached 70A even going super steep hill. Me 82kg + board ~20kg
```

---
## \#18 Posted by: E1Allen Posted at: 2018-04-19T20:56:55.899Z Reads: 44

```
What's your battery amps max per vesc?
```

---
## \#19 Posted by: Kug3lis Posted at: 2018-04-19T21:01:11.313Z Reads: 42

```
80A but I havent even reached 40 battery amp :)
```

---
## \#21 Posted by: mmaner Posted at: 2018-04-19T21:13:25.694Z Reads: 39

```
I don't ride as hard as you guys, but once when riding my evo in the dirt going uphill I hit 52a.  That's the highest I've ever been and I've tried to make it go higher and just can't.
```

---
