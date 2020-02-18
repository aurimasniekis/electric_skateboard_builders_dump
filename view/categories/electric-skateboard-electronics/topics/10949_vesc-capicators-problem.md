# Vesc Capicators Problem

### Replies: 30 Views: 2681

## \#1 Posted by: listgaus Posted at: 2016-10-11T08:02:16.616Z Reads: 191

```
Hey guys, 

I've been riding the Torqboards setup i purchased from diyelectricskateborads for a month now and yesterday when i plugged in my battery (6s lipo) via XT90 to the vedder vesc @chaka  i heard a small spark sound and the vesc didnot turn on.

i've checked visually and figured there is no damage to the vesc itself and after reading here a bit i figured i should test the votlage before and after the capacitor box, and what do you know?! the read before the capacitor is good (24 volts for my 6s 70% charged) and 0 volts after the capacitors....

This is bitter sweet since for once i was very dissapointed with my vesc faulting on me so fast but 2ndly i was happy to realize its the capacitors and that this vesc could be saved.

Question is, how to i solve this safely? can i go to an electric shop and get new capacitors of some kind and rewire them trough? 
Any suggestions? 

I'll be posting the thrilling video of my issue soon
```

---
## \#2 Posted by: Jakebarnhill1 Posted at: 2016-10-11T08:43:49.730Z Reads: 186

```
 If the VESC is receiving 0 volts there may be a faulty solder joint or something on the capacitor board like a broken copper trace, the capacitors are in parallel with the battery and are only there to smooth out the voltage ripples or spikes going into the battery, so if there is something wrong with the capacitors the esc should be still getting voltage unless there is a short, which you would definitely know about! I would carefully examine the capacitor board and solder joints and check for anything wrong. I hope this helps.
```

---
## \#3 Posted by: listgaus Posted at: 2016-10-11T09:29:32.558Z Reads: 173

```
I've uploaded the video, attached link here

https://sendvid.com/lobywqmi

i did a visual check on the capacitors, they look well in all connection point but when checking the outlet from them to the vesc there is no current passing.
```

---
## \#4 Posted by: flatsp0t Posted at: 2016-10-11T09:39:59.680Z Reads: 166

```
Check the traces on the PCB where the caps are soldered on.
If there are any Burn marks on it, it may be the easiest to just change the complete capPCB
```

---
## \#5 Posted by: listgaus Posted at: 2016-10-11T09:46:41.905Z Reads: 162

```
<img src="/uploads/db1493/original/3X/a/0/a05cdef3d65c1ef250df72831106cf0113c22812.jpg" width="281" height="500"> didnt spot anything burnt
```

---
## \#6 Posted by: listgaus Posted at: 2016-10-11T10:19:00.033Z Reads: 154

```
update

ive attached a one cell 3.6 battery to the output of the capacitor board and there is one blinking blue light from the vesc yet it is not recognized by the pc.

https://sendvid.com/eedfhnwa


any toughts?
```

---
## \#7 Posted by: Blasto Posted at: 2016-10-11T12:00:30.097Z Reads: 146

```
Check the impedance of the 3.3V rail and 5V. My guess is you have a low impedance on the 3.3v
```

---
## \#8 Posted by: listgaus Posted at: 2016-10-11T14:44:16.870Z Reads: 136

```
@blasto im not sure how to do that, can you explain on the vesc pic maybe?
and lets assum your right, whats the solution?
```

---
## \#9 Posted by: Blasto Posted at: 2016-10-11T14:55:27.491Z Reads: 144

```
[quote="listgaus, post:8, topic:10949"]
lets assum your right, whats the solution?
[/quote]
Need to send it in for repair... should be fairly easy fix. where are you located?

[quote="listgaus, post:8, topic:10949"]
im not sure how to do that,
[/quote]

Take a multimeter, put it in impedance (resistance, Ohm) check the 5V to gnd and the 3.3V to gnd. while the vesc is powered off. Both voltage rail should be identified on the silkscreen near the connectors.
```

---
## \#10 Posted by: listgaus Posted at: 2016-10-11T15:49:53.868Z Reads: 140

```
If i understood correctly, than the read for the 3.3 on 200k ohm resistance 0.1 and on the 5v is 15.2 

is that it?


and im from israel, if its an easy fix maybe i could do it myself?

<img src="/uploads/db1493/original/3X/a/1/a1be9e760a9d211e8d6ed29e64c1f09cf2612c0f.jpg" width="281" height="500">
```

---
## \#11 Posted by: Blasto Posted at: 2016-10-11T16:13:10.811Z Reads: 132

```
[quote="listgaus, post:10, topic:10949"]
If i understood correctly, than the read for the 3.3 on resistance 0.1 
[/quote]

You have a short circuit on the 3.3V rail, most common component that is prone to fail in this case is the can transceiver, U401.

If you are able to remove it (without destroying everything), measure again, you'll notice a much higher resistance
```

---
## \#12 Posted by: listgaus Posted at: 2016-10-11T16:43:02.355Z Reads: 120

```
im afraid im incapable of doing so. is that the only solution? removing/replacing it?
```

---
## \#13 Posted by: listgaus Posted at: 2016-10-11T16:44:06.840Z Reads: 121

```
[quote="Blasto, post:11, topic:10949"]
If you are able to remove it (without destroying everything), measure again, you'll notice a much higher resistance
[/quote]

im afraid im incapable of doing so. is that the only solution? removing/replacing it?
```

---
## \#14 Posted by: Blasto Posted at: 2016-10-11T16:53:48.864Z Reads: 119

```
Well the more destructive method would be to use some flush cutters and clip each leg of U401 off... Then again, i'm not 100% sure that this is your problem.
```

---
## \#15 Posted by: listgaus Posted at: 2016-10-11T17:06:39.247Z Reads: 117

```
so who you said could help? :confused:
```

---
## \#16 Posted by: flatsp0t Posted at: 2016-10-11T18:22:22.761Z Reads: 120

```
maybe you need to ship it back to @torqueboards.
```

---
## \#17 Posted by: zmoney Posted at: 2016-10-12T00:57:21.838Z Reads: 121

```
Looks like you're missing a cap at C26

<img src="/uploads/db1493/original/3X/a/e/ae233fdd129f4a172c8fb0406c9567cb469a785c.JPG" width="690" height="374">
```

---
## \#18 Posted by: JohnnyMeduse Posted at: 2016-10-12T01:09:22.844Z Reads: 118

```
well it is not really relevant, it for FOC purpose and had been added on the 4.12 version. So @Torqueboard probably use the 4.10BOM on 4.12 PCB, nothing to really worry about except for FOC.
```

---
## \#19 Posted by: JohnnyMeduse Posted at: 2016-10-12T01:16:57.366Z Reads: 117

```
also try this to check the can tranceiver

http://www.electric-skateboard.builders/t/no-power-to-enertion-vesc/7600/8?u=johnnymeduse
```

---
## \#20 Posted by: listgaus Posted at: 2016-10-12T07:30:55.085Z Reads: 105

```
[quote="JohnnyMeduse, post:19, topic:10949"]
also try this to check the can tranceiver
[/quote]

I did the test you showed, the results are that i get a steady current on the c25 as you can see in the video
and when diods touch eachother they go wild and unsteady

https://vid.me/E1zG

what do you think?
```

---
## \#21 Posted by: JohnnyMeduse Posted at: 2016-10-12T12:39:09.563Z Reads: 88

```
In diode check mode, when you have a short it is suppose to show 000, but if you have over 150 it's ok, that just mean that you don't have a short over the Can Tranceiver U401... Now, if you can just check the continuity (for the black and the red wire) from your battery connector to the pads on the PCB, to see if you have a bad connection over the capacitor board. (because for what I've see from Torqueboards VESC the soldering on the capacitor board is not really good).
```

---
## \#22 Posted by: listgaus Posted at: 2016-10-12T15:58:18.556Z Reads: 82

```
if i understood right here are the results. sorry but the host site has somehow flipped the view 180 degrees

http://sendvid.com/cybkpk74
```

---
## \#23 Posted by: JohnnyMeduse Posted at: 2016-10-12T16:48:16.120Z Reads: 80

```
It is ok to see some variation when the current is passing trough the capacitor. Buy from what a can see in your video I'am confident to tell your that you have a bad soldering over de ground wire... You will need to re-soldering it or contact @torqueboards to figure out orther option... Or I can do it for you but I'm located a bit far. (Canada)
```

---
## \#24 Posted by: listgaus Posted at: 2016-10-12T17:03:38.527Z Reads: 79

```
thanks. i have a solder if its not something too too tricky. soldering from the side where it's writted "vedder capacitor board" should do?
```

---
## \#25 Posted by: JohnnyMeduse Posted at: 2016-10-12T17:26:35.784Z Reads: 74

```
No, just resolder de power cable on capacitor board and test it again
```

---
## \#26 Posted by: listgaus Posted at: 2016-10-12T18:09:09.502Z Reads: 70

```
[quote="JohnnyMeduse, post:25, topic:10949"]
just resolder de power cable on capacitor board and test it again
[/quote]

did it, getting 00.2 on the read from the side of the output to the vesc :confused:
```

---
## \#27 Posted by: JohnnyMeduse Posted at: 2016-10-12T18:25:19.918Z Reads: 70

```
What is at 0.000 volt or on diode check?
```

---
## \#28 Posted by: listgaus Posted at: 2016-10-12T18:31:00.211Z Reads: 68

```
[quote="JohnnyMeduse, post:27, topic:10949, full:true"]
What is at 0.000 volt or on diode check?
[/quote]

the power cables (red and black) on the vesc
```

---
## \#29 Posted by: JohnnyMeduse Posted at: 2016-10-13T03:32:18.670Z Reads: 60

```
ok, so it is looking like a bad capacitor board, your best bet will be to contact @torqueboards to see if he can propose you any solution for the repair.
```

---
## \#30 Posted by: Mike_Lemon Posted at: 2017-04-04T13:14:31.608Z Reads: 42

```
Hello, listgaus.

Did you fix that problem? I've also encountered it and I managed to find out how to fix it.
I'm also from Israel so maybe we could talk.
```

---
