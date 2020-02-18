# VESC Motor Connections

### Replies: 12 Views: 3090

## \#1 Posted by: treenutter Posted at: 2015-09-25T17:56:19.510Z Reads: 203

```
Some folks wire their motor wires directly to the VESC, which seems fine. I've noticed that some, however, have these connectors that they solder to the board instead of a wire. This is an image I 'capped from one of @onloops's videos:

<img src="/uploads/db1493/original/1X/78ab373678730fc63cc2089fc55eac32b3a5b397.png" width="690" height="444"> 

Those red, yellow, and blue connectors; what are they? Are they a special right-angled 4mm bullet connector? Is it possible to solder a whole, regular, 4mm bullet connector right onto the VESC board?
```

---
## \#2 Posted by: lox897 Posted at: 2015-09-25T17:58:51.767Z Reads: 198

```
@sl33py Knows how to do this.
```

---
## \#3 Posted by: lox897 Posted at: 2015-09-25T18:00:40.222Z Reads: 196

```
I think you put some solder on one side of the connector and place it vertically. I am not sure if this is the way to do it though.
```

---
## \#4 Posted by: lox897 Posted at: 2015-09-25T18:08:06.097Z Reads: 195

```
<img src="/uploads/db1493/original/1X/f217185ab304c4cce2dc0cb41e0e944850da8423.jpg" width="318" height="500"> 

Here's a better photo
```

---
## \#5 Posted by: lowGuido Posted at: 2015-09-25T18:12:32.504Z Reads: 190

```
I believe they are a pretty standard 5mm bullet connector just dremeled out at the end.
```

---
## \#6 Posted by: torqueboards Posted at: 2015-09-25T18:55:05.285Z Reads: 189

```
They have these 5.5mm bullet connectors which have a part that you can put over the edge of the board. Then just use enough solder.

<img src='/uploads/db1493/original/1X/e4ec750ad1f4987fa0942f7396dd7ca91e5f09ba.jpg'>

The actual color is just from the heatshrink wrap.

At least that's how I'd do it.

You could possibly cut pieces of the standard 5.5mm connectors to make them like the one above.
```

---
## \#7 Posted by: treenutter Posted at: 2015-09-25T19:09:01.432Z Reads: 179

```
Thanks @lox897 @torqueboards @lowGuido. I was hoping there was an L-shaped bullet connector out there somewhere! I was thinking that there is some value to keeping the motor wires modular. Then they can be easily shortened or extended without having to desolder from the pcb. 

Any thoughts on using a very short wire for the motor connectors on the VESC, perhaps 3cm? (so it would be wire soldered to the board, a short wire, and then a bullet) Then some extensions (12AWG, 4mm bullet) to reach the mounted motor connectors? I'm unsure of the impact of adding another connector into the chain, and that's not how Vedder does it :smile:
```

---
## \#8 Posted by: lowGuido Posted at: 2015-09-25T19:09:18.913Z Reads: 176

```
the ones in the picture lox posted are soldered on both sides, so there would have to be a slot cut to allow the PCB to slide in the middle and have solder both sides.
```

---
## \#9 Posted by: lowGuido Posted at: 2015-09-25T19:13:56.064Z Reads: 179

```
you can add as many connectors as you want. I try to avoid it because it just ads another possible thing to come un plugged, but its all up to you. there is no wrong way to build an e board. 

personally if it was me, id probably solder on the 4mm bullets that match the motor so that you can just plug the motor direct to the ESC.
```

---
## \#10 Posted by: treenutter Posted at: 2015-09-25T19:17:46.753Z Reads: 173

```
Thanks @lowGuido, I agree; I've got the 4mm bullets to use. I'll need to extend them somehow; I don't think the motor wires will reach the VESC otherwise.
```

---
## \#11 Posted by: lowGuido Posted at: 2015-09-25T19:20:08.672Z Reads: 171

```
yeah well if the ESC is too far away then you have no choice but to extend them.
```

---
## \#12 Posted by: onloop Posted at: 2015-11-15T20:58:59.394Z Reads: 146

```
5 posts were split to a new topic: [What order should I connect the 3 Motor wires to the ESC](/t/what-order-should-i-connect-the-3-motor-wires-to-the-esc/487)
```

---
