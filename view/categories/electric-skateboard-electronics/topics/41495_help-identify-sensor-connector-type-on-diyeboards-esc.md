# Help identify sensor-connector type on Diyeboards esc

### Replies: 19 Views: 1639

## \#1 Posted by: leven Posted at: 2017-12-19T22:14:29.684Z Reads: 170

```
Hi,

i was going to try and add a sensor to an unsensored motor so i bought a couple of hall sensors from alienpowersystem:
http://alienpowersystem.com/shop/brushless-motors/50mm/internal-pcb-with-hall-effect-sensors-120-degree/

But of course the connector was different on the ESC, and i need help identifying it.

Its the one on the ESC i would like, from this one:
http://www.diyeboard.com/v11-dual-belt-motor-sine-wave-foc-esc-speed-controller-p-522.html

Have been looking at JST-connectors but there's a lot of them, anyone who knows what model i need?
I measured the connector on the inside, it's 4mm in height, 10,7mm width and the pins are 2mm apart.
```

---
## \#2 Posted by: Martinsp Posted at: 2017-12-19T22:43:45.769Z Reads: 149

```
Search eBay for jst 2.0 and just find the right number of pins and male/female. It should be easy to find jst connectors are fairly standard.
```

---
## \#3 Posted by: Kug3lis Posted at: 2017-12-19T22:47:43.238Z Reads: 138

```
P.S. I think those sensors boards are meant for APS motors, because of design, but maybe you will be able to adapt them.
```

---
## \#4 Posted by: leven Posted at: 2017-12-19T22:57:47.561Z Reads: 132

```
Ok, its that easy? I thought it was a lot of different jst connectors, but thanks, will do!
```

---
## \#5 Posted by: leven Posted at: 2017-12-19T23:04:17.353Z Reads: 115

```
Yeah i figured, but i epoxied it to a stator of an unsensored motor i had picked apart, it's more of a fun test to see if it works..
```

---
## \#6 Posted by: Martinsp Posted at: 2017-12-19T23:10:15.151Z Reads: 107

```
It will work, I have modified a couple of motors this way. I even just glued some sensors between the stator teeth and it worked nicely. 

There is many jst connectors for example with locks etc but these are the standard type
```

---
## \#7 Posted by: deucesdown Posted at: 2017-12-19T23:15:25.580Z Reads: 105

```
[quote="leven, post:1, topic:41495"]
pins are 2mm apart
[/quote]


That should be JST-PH
```

---
## \#8 Posted by: leven Posted at: 2017-12-19T23:19:21.026Z Reads: 99

```
[quote="deucesdown, post:7, topic:41495"]
JST-PH
[/quote]

Thank you, made the search easier.
```

---
## \#9 Posted by: rey8801 Posted at: 2018-03-08T08:26:32.298Z Reads: 72

```
Hi, did you figure it out how to connect them? I would be interested in knowing which is the pin order on the ESC for the sensor cable. I know you should have 5 cables and it is importat to place correctly the 5v and the ground ones (usally red and black, but I want to be sure). Thx for the help!
```

---
## \#10 Posted by: leven Posted at: 2018-03-11T21:34:05.206Z Reads: 58

```
Hi, no I did end up switching the esc for a couple of vescs i already had.

The order was easy, the first and last was 5V and gnd, the other three where marked.

But I think the problem was that the diyeboard esc had different angled phase sensors so it did not sense my motors.

 That's why the vesc, there you can adjust for that.
```

---
## \#11 Posted by: rey8801 Posted at: 2018-03-11T22:29:09.486Z Reads: 56

```
Thanks for the information. You said the other three were marked but where you see the order for the green, blue and yellow? If you can post a picture about it would help a lot! Thx
```

---
## \#12 Posted by: scepterr Posted at: 2018-03-11T22:35:31.803Z Reads: 52

```
Order of sensors didn't matter for mine, just plugged in and it ran, if a motor is spinning the wrong direction switch two phase wires
![IMG_20180226_232427|450x500](upload://7STHZT1KZdsqjiiQiV3TbLZieB3.jpg)
```

---
## \#13 Posted by: rey8801 Posted at: 2018-03-11T22:40:05.047Z Reads: 51

```
I though that also the sensor wires as to be ordered based on the phase wire. Othersiwe how can they now which sensor is ocnnected with what?
```

---
## \#14 Posted by: leven Posted at: 2018-03-11T22:43:22.281Z Reads: 52

```
They where marked on the esc and on the sensor-boards I got from alienpowersystems.

The motors worked but they where not sensored, and where still stuttering on startup.
```

---
## \#15 Posted by: scepterr Posted at: 2018-03-11T22:47:08.411Z Reads: 51

```
I just kept the same order the 6 pin connector had when switching to 5 pin and kept phase leads in order 1,2,3 left to right and kept the order coming out of the esc , just worked
https://youtu.be/GP62E0CwZec
```

---
## \#16 Posted by: rey8801 Posted at: 2018-03-12T05:53:18.442Z Reads: 48

```
By the pictures available online I can not read a thing on the ESC. Would you mind to take a picture of the ESC where you can see it? The reason why of that is bacause I need to link the sensor wire to a VESC. Thx
```

---
## \#17 Posted by: leven Posted at: 2018-03-14T10:22:30.399Z Reads: 44

```
![esc1|375x500](upload://qmrfOJvHU68OBfyCo6Pmbm1MEQM.jpg)![esc2|375x500](upload://dPeY4IU6p5HoFwJ6TBla02TCnBU.jpg)

Hi, these are two pictures of the ESC, one where you see the markings and one with the sensor connector from a diyebord-motor (90mm hub motor) plugged in.
```

---
## \#18 Posted by: rey8801 Posted at: 2018-03-14T10:56:26.522Z Reads: 39

```
Awesome! Thanks a lot...
```

---
## \#19 Posted by: lcoigrta Posted at: 2019-03-21T15:38:03.017Z Reads: 14

```
![received_1032833796903176|279x500](upload://lfKf2l0ckoeNp6qeq21HNPT2Xin.jpeg) ![received_383139185605628|279x500](upload://mWdrpNzQz49lGQG4Q3sEL4ry2cr.jpeg) what jst connector is that?
```

---
