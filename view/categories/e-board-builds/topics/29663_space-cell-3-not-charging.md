# Space cell 3 not charging

### Replies: 31 Views: 1058

## \#1 Posted by: joeadams101 Posted at: 2017-08-04T06:53:31.822Z Reads: 71

```
I am curious about the reasons why a space cell 3 wont charge. Its at 13%. When I connect the charger it jumps to 100% and the light on the charger stays green. Thoughts?
```

---
## \#2 Posted by: Bloop Posted at: 2017-08-04T08:42:09.886Z Reads: 60

```
Hard to say.. you will need to provide more informations maybe some pics or a video

Have you checked the wires ?
```

---
## \#3 Posted by: ElskerShadow Posted at: 2017-08-04T08:58:19.699Z Reads: 59

```
Yeah hard to say with not so much info. My bet is something is not well soldered I had several problem milke this with mine. I re did all the solder job and it was fine
```

---
## \#4 Posted by: Jebe Posted at: 2017-08-04T09:40:16.622Z Reads: 53

```
do you have a voltage meter? Disconnect the charger and measure the voltage across the vesc.
```

---
## \#5 Posted by: joeadams101 Posted at: 2017-08-04T14:54:37.872Z Reads: 40

```
Hey guys I took the battery out from the case and started checking everything. I found out that when i adjusted a cable and connected the charger it started charging! The light turn red. What do yoy guys think I should do? Here are the pictures showing what cable I am talking about. <img src="/uploads/db1493/original/3X/0/a/0aa41423ce5066cf57b68cc1bf723be4ff50e42e.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/d/d/dd3bbcebe805e2198e7612a87c72bb58d18698a6.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/7/b7b9d1636286670c602c61a32d6b86fb63c1e807.jpg" width="690" height="388">
```

---
## \#6 Posted by: melchiorvester Posted at: 2017-08-04T15:04:23.745Z Reads: 37

```
Could be a dead row of cells in that parallel
```

---
## \#7 Posted by: joeadams101 Posted at: 2017-08-04T15:06:02.171Z Reads: 37

```
Its charging now. I will update when it finished charging. Hopefully to 100% since there are no broken cables around.
```

---
## \#8 Posted by: joeadams101 Posted at: 2017-08-04T16:07:27.549Z Reads: 36

```
Update: so it fully charged but the light on the charger was still red. Unplugged the charger and it stayed at its current battery percentage. Connected my vesc and motor and receiver and seems to be working fine. Now...how do I fix that cable? If its moved drastically it will cause to not charge and go to 100% when the charger is connected(while the actually battery is maybe 60 75 or any number..)
```

---
## \#9 Posted by: Jinra Posted at: 2017-08-04T16:19:29.599Z Reads: 34

```
Are you saying if you adjust the cable in the picture (battery negative) it causes it to charge/not charge? If it's that cable you can unsolder and resolder. I would check to see where exactly the problem is though. Perhaps it's a loose connection or the nickel strip is breaking.
```

---
## \#10 Posted by: joeadams101 Posted at: 2017-08-04T16:31:43.414Z Reads: 31

```
@Jinra hey Jinra! So when I first opened the battery jt bad some broken connections (2). Soldered them...That did not fixed the problem. I starting checking everything making sure nothing was loose. I turned the battery on then started moving cables again...nothing happened until i moved that battery negative cable i saw the percentage go to its actual charge. Then i connected the charger and it started charging. My guess that cable is the problem. Correct me if I am wrong
```

---
## \#11 Posted by: Jinra Posted at: 2017-08-04T16:33:23.446Z Reads: 30

```
Sounds like it, try wiggling it around to see if it has a poor connection anywhere or if the nickel strip is breaking. Also check both ends.
```

---
## \#12 Posted by: joeadams101 Posted at: 2017-08-04T16:40:22.315Z Reads: 30

```
Yeah so when I wiggled it you can see the percentage on the battery goes to 10% and it doesnt charge. When u move it a certain direction it goes back to normal. But when u wiggle it randomly u see the percentage going up and down.
```

---
## \#13 Posted by: Jinra Posted at: 2017-08-04T16:43:38.953Z Reads: 29

```
cool so just resolder the connection and you should be good
```

---
## \#14 Posted by: joeadams101 Posted at: 2017-08-04T16:45:22.703Z Reads: 27

```
Thats what I am going to do when I get home tonight. I will keep you guys updated.
```

---
## \#15 Posted by: Bensaida Posted at: 2017-08-05T00:14:28.439Z Reads: 26

```
Any luck with it bro?
```

---
## \#16 Posted by: joeadams101 Posted at: 2017-08-05T02:24:56.311Z Reads: 23

```
Okay guys so i tried resoldering the cable and no luck i did notice a strange behavior . Take a look and tell me what you think.

https://youtu.be/07EM5nfRcS4
```

---
## \#17 Posted by: Bloop Posted at: 2017-08-05T02:37:19.306Z Reads: 21

```
This looks like a bad connection. Since when you move it around it is working ok and in some other position it dose not.

If you have a multimeter just test each end of the cells to see where the problem is.
```

---
## \#18 Posted by: joeadams101 Posted at: 2017-08-05T02:40:19.882Z Reads: 21

```
What would be consider the end of the cells? Also should I test out the components in the front ? Like the bms and all that? I am going to get a multimeter now..
```

---
## \#19 Posted by: Bloop Posted at: 2017-08-05T02:46:09.183Z Reads: 22

```
First of all i would test the overall voltage of the battery. The Black wire and the red wire that is at very end of you battery. 

If this voltage is good then go check on other components like bms.. If you dont get your full voltage at the ends you need to go and check every single little cell from end to end and see what is the voltage on each one. If they are all in good shape then check every group of 3 if is connected with the next one and i assume you will find somewhere a loose connection.

Good luck hope this helps
```

---
## \#20 Posted by: Jinra Posted at: 2017-08-05T02:55:50.175Z Reads: 22

```
As @Bloop said, probe the output terminals with a multimeter to read voltage. Then move the pack around like in the video and see if that reading changes at all. It may just be a faulty meter or connection to the meter.
```

---
## \#21 Posted by: joeadams101 Posted at: 2017-08-05T03:09:45.447Z Reads: 22

```
Okay just got this off a store. Anyone can guide me on the settings I need to plug?<img src="/uploads/db1493/original/3X/4/4/449a5ea576c47b1ffb5c2f7463c1da5fce0eb6e8.jpg" width="243" height="500">
```

---
## \#22 Posted by: Jinra Posted at: 2017-08-05T03:16:15.053Z Reads: 21

```
Flip it to DCV 200

Plug black probe into COM port
Plug red probe into the one above it
```

---
## \#23 Posted by: joeadams101 Posted at: 2017-08-05T03:24:45.069Z Reads: 20

```
Got it. Sorry never done this before. Where do I put it to test the<img src="/uploads/db1493/original/3X/0/a/0aa41423ce5066cf57b68cc1bf723be4ff50e42e.jpg" width="690" height="388"> battery out?

If u can point it out in this pic that will be awesome
```

---
## \#24 Posted by: Jinra Posted at: 2017-08-05T03:31:51.216Z Reads: 19

```
the plug that goes to the VESC, red to red, black to black.

Don't short the probes
```

---
## \#25 Posted by: joeadams101 Posted at: 2017-08-05T03:49:18.277Z Reads: 18

```
Okay let me try it. Do the battery has to be on?
```

---
## \#26 Posted by: Jinra Posted at: 2017-08-05T03:50:02.835Z Reads: 18

```
yes of course
```

---
## \#27 Posted by: joeadams101 Posted at: 2017-08-05T03:52:43.345Z Reads: 18

```
Giving me 35.5 even when the percentage goes down on the  lcd panel of battery it stays at 35.5
```

---
## \#28 Posted by: Jinra Posted at: 2017-08-05T03:54:04.192Z Reads: 18

```
Now probe around some more on the meter cable to try and find out if it's the wires or the meter itself.
```

---
## \#30 Posted by: joeadams101 Posted at: 2017-08-05T03:55:59.391Z Reads: 17

```
Which are those?
```

---
## \#31 Posted by: joeadams101 Posted at: 2017-08-05T03:56:38.759Z Reads: 18

```
<img src="/uploads/db1493/original/3X/0/b/0b7a96a3bf0230ae3b2f7eda8707686f5fe54e22.jpg" width="281" height="500">
```

---
## \#32 Posted by: Jinra Posted at: 2017-08-05T03:56:58.221Z Reads: 19

```
The red and black cable coming from the meter
```

---
