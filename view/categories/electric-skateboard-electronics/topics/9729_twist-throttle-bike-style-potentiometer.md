# Twist throttle &lsquo;bike style&rsquo; Potentiometer

### Replies: 27 Views: 3349

## \#1 Posted by: barajabali Posted at: 2016-09-17T02:54:48.204Z Reads: 287

```
Any one know how to get a hard wired pretentiometer for an e-skate? Or a push throttle. I want to hard wire my mountain board since I'm putting some disc brakes on it. I'm not sure what I'll need for this project. 

Links help a lot! :)  is there a thumb throttle that just plugs into the esc possibly? Who knows

https://www.ebay.com/itm/232031220144  Maybe like this? And just direct solder it to the esc? I'm using the TB esc and that needs a ubec so I think that would play a role too...
```

---
## \#2 Posted by: cmatson Posted at: 2016-09-17T03:22:25.690Z Reads: 278

```
Fing disk brakes?? 

You could try hacking up an rc servo tester - they are just like little receivers with a potentiometer for moving your servo or throttle range to calibrate an rc car. 

Maybe you could use that for the pcb board, and just buy a twist throttle potentiometer that can be wired instead of the stock little servo tester knob.
```

---
## \#3 Posted by: cmatson Posted at: 2016-09-17T03:24:37.482Z Reads: 259

```
By the way, I used the same throttle you linked to fix up a craigslist ground force drifter (razor go kart thing) for one of my little bros. It's worked really well for the last year or so, even repeatedly getting caught in the rain and stuff..
```

---
## \#4 Posted by: barajabali Posted at: 2016-09-17T03:27:14.107Z Reads: 243

```
Yes disk brakes I've had too many close calls on my board I need some mechanical brakes to come to a full stop as I can jump off. 

And I want the thumb thrilled to install onto the hand brake so it's all on one hand. 

I don't have experience with servo testers but that could be an option. 

You don't think direct soldering that throttle to the esc wire would work right? And wire a ubec in line
```

---
## \#5 Posted by: anon33082420 Posted at: 2016-09-17T03:51:59.320Z Reads: 231

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#6 Posted by: psychotiller Posted at: 2016-09-17T03:54:06.688Z Reads: 227

```
You should buy a Wiiceiver from Torqueboards and then just plug in a wired nunchuck. Works perfectly and you'd have cruise control.
```

---
## \#7 Posted by: Blasto Posted at: 2016-09-17T04:14:54.393Z Reads: 219

```
Just wire it up to to the adc input of the vesc. Make sure your pot is on the 3.3v.

So in your case "positive electrode" to 3.3V, "signal" to adc 1 and gnd to gnd.


Setup the vesc in the analog tab
```

---
## \#8 Posted by: saul Posted at: 2016-09-17T04:27:31.322Z Reads: 219

```
Those bike throttles usually use a hall sensor so it probably wont work directly, and they only have a forward direction not back twist for regen, guess its ok if you only use the disks...

I would take a pot from a quantum/gt2b or something and wire it to the vesc like blasto suggested, but not experience with this setup, Should be no lag!
```

---
## \#9 Posted by: anon33082420 Posted at: 2016-09-17T04:28:31.833Z Reads: 211

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#10 Posted by: Okami Posted at: 2016-09-17T08:32:03.199Z Reads: 189

```
http://www.electricscooterparts.com/throttles.html

Maybe this helps.

motorcycle / scooter type electronic throttles
```

---
## \#11 Posted by: barajabali Posted at: 2016-09-17T13:19:53.562Z Reads: 177

```
Okay so i need the servo tester and the item you linked and I should be good?
```

---
## \#12 Posted by: barajabali Posted at: 2016-09-17T13:22:57.530Z Reads: 175

```
Ohhhhh I get it. Thanks guys and @LEVer

I just need to wire the esc to the servo tester and then swap out the knob on the tester with the throttle wires.  and ubec goes to the tester too.c
```

---
## \#13 Posted by: cmatson Posted at: 2016-09-17T16:29:26.993Z Reads: 168

```
[quote="barajabali, post:12, topic:9729"]
I just need to wire the esc to the servo tester and then swap out the knob on the tester with the throttle wires
[/quote]

yep, that's what I was thinking-
```

---
## \#14 Posted by: anon33082420 Posted at: 2016-09-17T16:58:03.612Z Reads: 158

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#15 Posted by: barajabali Posted at: 2016-09-17T19:27:08.658Z Reads: 153

```
Well I'm gonna buy the disc brakes from trampa and swap out the cable and handle. (Hopefully) 

You think it'll work?
```

---
## \#16 Posted by: flatsp0t Posted at: 2016-09-17T20:52:24.393Z Reads: 151

```
It would work propably, but beware trampa uses hydraulic brakes, so it is a bit more difficult.
```

---
## \#17 Posted by: anon33082420 Posted at: 2016-09-17T21:11:02.316Z Reads: 146

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#18 Posted by: barajabali Posted at: 2016-09-17T23:59:23.167Z Reads: 146

```
Hmmm that's a challenge...  I suppose I could remove brakes on the esc and that may solve the issue. Either turn brakes down to 10% or try to deactivate them all together.
```

---
## \#19 Posted by: barajabali Posted at: 2016-09-17T23:59:57.609Z Reads: 152

```
It's so funny how making a hard wire connection is actually harder than wireless
```

---
## \#20 Posted by: anon33082420 Posted at: 2016-09-18T01:17:42.656Z Reads: 154

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#21 Posted by: JLabs Posted at: 2016-09-18T02:04:35.064Z Reads: 143

```
I was actually wondering the same thing. I want to add physical brakes to my MTB (when I build it) so I can bomb hills and paths and not worry about damaging the motor or the brakes giving out. What about hardwiring a wii kama? You would have the nunchuck style control (which I prefer) but there would be no easy way to make it twist throttle.
```

---
## \#22 Posted by: anon33082420 Posted at: 2016-09-18T02:16:09.211Z Reads: 142

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#23 Posted by: saul Posted at: 2016-09-19T07:14:10.865Z Reads: 130

```
you could stick the servo tester inside the eglide remote and connect the trigger pot to the servo tester pot pins...then you still have regen for better speed control, and disks to stop.

Then you just have to figure out how to add the brake lever...
```

---
## \#24 Posted by: lowGuido Posted at: 2016-09-19T09:29:48.928Z Reads: 130

```
you could always use the VESC's built in twist throttle compatibility..

( edit: @blasto did mention this above)
```

---
## \#25 Posted by: psychotiller Posted at: 2016-09-20T03:02:52.636Z Reads: 119

```
The twist throttle I put on Aedens kickboard rests in neutral. 
https://youtu.be/q9eoc562kcw
```

---
## \#26 Posted by: Obiben Posted at: 2018-05-01T02:09:43.707Z Reads: 62

```
Hey @psychotiller , I know this is old-ish, but do you happen to know where you found the T-bar and what twist throttle this is?

I'm looking to make something exactly like this and am really to sure what to look for and where!
```

---
## \#27 Posted by: psychotiller Posted at: 2018-05-01T03:50:12.105Z Reads: 52

```
The T handle was made for me at rogers bros downhill. and the twist throttle i bought on ebay.

You'll also need to hook the throttle up to the adc pinouts on the vesc.
```

---
