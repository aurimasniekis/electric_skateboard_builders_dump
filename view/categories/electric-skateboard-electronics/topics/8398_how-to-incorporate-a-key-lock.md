# How to incorporate a Key Lock

### Replies: 25 Views: 1679

## \#1 Posted by: anorak234 Posted at: 2016-08-26T22:50:25.651Z Reads: 172

```
I have been thinking about getting this lock switch to use as the on/off switch on my latest build: https://www.amazon.com/gp/aw/d/B0002BA3PE/ref=cm_cr_arp_mb_bdcrb_top?ie=UTF8 
I don't know if the switch can handle the current, how would I get around that?
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-08-26T22:51:05.130Z Reads: 170

```
I've used one similar before, it should be fine.
```

---
## \#3 Posted by: mason Posted at: 2016-08-26T23:35:18.542Z Reads: 157

```
Use it with an antispark switch and have it be the on/off button.
```

---
## \#4 Posted by: anorak234 Posted at: 2016-08-26T23:47:57.736Z Reads: 151

```
Sounds good, does anybody know the dimensions of these? The Amazon one doesn't seem to be accurate, there's no way that thing is 3 X 3 inches
```

---
## \#5 Posted by: JLabs Posted at: 2016-08-26T23:50:47.755Z Reads: 140

```
I don't want to be a bummer, but what is his going to do?
```

---
## \#6 Posted by: anorak234 Posted at: 2016-08-27T00:03:57.949Z Reads: 138

```
1) stop my friends from taking my board out all the time because they don't want to build or buy one
2) if someone steals it that doesn't know what they're doing, they won't be able to turn it on
```

---
## \#7 Posted by: JLabs Posted at: 2016-08-27T00:07:59.332Z Reads: 133

```
Ahh, ok ok. I could see this being the external with for the antispark (bedder). Now that would be hella cool.
```

---
## \#8 Posted by: anorak234 Posted at: 2016-08-27T00:12:39.258Z Reads: 133

```
Do you happen to have a diagram? I am struggling to figure out how I would solder it with an antispark...
```

---
## \#9 Posted by: Namasaki Posted at: 2016-08-27T00:24:36.383Z Reads: 135

```
Another option that will solve the key and anti spark situation is to use a xt90 anti-spark  loop connector.
Just mount the female socket on your enclosure so you can plug and unplug the loop connector outside the enclosure.

http://www.hobbyking.com/hobbyking/store/__61690__XT90_S_Anti_Spark_Connector_2pairs_bag_.html
```

---
## \#10 Posted by: sl33py Posted at: 2016-08-27T00:28:38.872Z Reads: 132

```
was thinking something like this as a battery disconnect:
https://www.amazon.com/Perko-8502DP-Locking-Battery-Selector/dp/B000KOU7ZO
```

---
## \#11 Posted by: mason Posted at: 2016-08-27T00:35:57.005Z Reads: 120

```
http://ih0.redbubble.net/image.195024098.5417/flat,1000x1000,075,f.jpg

using it on a vedder switch or something. this will open/close the power switch circuit
```

---
## \#12 Posted by: Namasaki Posted at: 2016-08-27T00:36:03.557Z Reads: 111

```
Those are designed for 12v and will wear out from internal spark.
```

---
## \#13 Posted by: sl33py Posted at: 2016-08-27T00:45:51.159Z Reads: 104

```
For use with systems under 50 volts. capacity - 250 amps continuous, 360 amps Intermittent.
```

---
## \#14 Posted by: Namasaki Posted at: 2016-08-27T00:52:04.962Z Reads: 104

```
Ok, you right. They are a bit bulky though.
```

---
## \#15 Posted by: JohnnyMeduse Posted at: 2016-08-27T00:54:09.371Z Reads: 104

```
2.6 x 5.2 x 5.2 inches.... where can you put this on a board..
```

---
## \#16 Posted by: sl33py Posted at: 2016-08-27T00:54:20.922Z Reads: 105

```
Yup!  But a unique option w/ key and supposed to handle volts and amps we use.
```

---
## \#17 Posted by: anorak234 Posted at: 2016-08-27T01:13:23.565Z Reads: 103

```
<img src="/uploads/db1493/original/2X/f/f4fe8ccb7ef917f07e762ebeb62d21d586b85aa0.png" width="690" height="301">
correct?
```

---
## \#18 Posted by: mason Posted at: 2016-08-27T01:14:31.513Z Reads: 101

```
the MEB antispark has a push button, correct? If so, splice one of the wires from it and bridge it with the key switch.
```

---
## \#19 Posted by: anorak234 Posted at: 2016-08-27T01:16:17.790Z Reads: 105

```
This is the MEB switch, it has three wires:
<img src="/uploads/db1493/original/2X/e/e4e164cd8aa8dbf690a276c4c5aefa17d2240d1a.jpg" width="500" height="500">
```

---
## \#20 Posted by: JLabs Posted at: 2016-08-27T01:16:55.172Z Reads: 102

```
There is a solid wire coning from the anti to the esc. The switchboard separate conic off of the anti, as it's own 2 cables.
```

---
## \#21 Posted by: anorak234 Posted at: 2016-08-27T01:23:06.024Z Reads: 103

```
Ok so from what I understand, this is the way that the switch is set up:
<img src="/uploads/db1493/original/2X/0/0f37507faf952cb28743d6bc0c0829512abf9ef4.png" width="652" height="356">
It has one red, one black, and one yellow wire. 
This is what I think needs to happen? But then where does the yellow wire go?
<img src="/uploads/db1493/original/2X/3/3e4fa89f08f304964335d3faa11ebdc1197f7578.png" width="652" height="342">
```

---
## \#22 Posted by: mason Posted at: 2016-08-27T01:50:01.560Z Reads: 89

```
keep the push button.

cut the negative and bridge it with the key. that way, when the key is in ignition position all you need to do is press the button for the switch to activate. the key closes the circuit.
```

---
## \#23 Posted by: JLabs Posted at: 2016-08-27T01:59:34.955Z Reads: 90

```
You can keep the switch all ways on and inside your enclosure and split the black wire and wire it like a loop key. Then you know it will work, and it is the only thing on the outside of the enclosure.
```

---
## \#24 Posted by: Namasaki Posted at: 2016-08-27T04:00:49.797Z Reads: 85

```
The third wire is for the light in the switch button
```

---
## \#25 Posted by: KB1.0 Posted at: 2018-04-24T20:19:42.083Z Reads: 32

```
could i also use an aruino and an rfid reader instat of the button?
```

---
