# Power Glove Controller DIY (with video test ride)

### Replies: 13 Views: 2235

## \#1 Posted by: saul Posted at: 2016-10-06T08:07:40.929Z Reads: 307

```
So I was curios how bb made their controller so small, and the secret, no potentiometers! 
They use linear hall sensors. :nerd:

so a couple ss495b and [this example code for arduino](https://arduining.com/2012/07/17/arduino-hall-effect-sensor-gaussmeter/), + my awesome neff snowboard gloves....

I think It would be really nice to wear gloves now that its getting cold, and this is just LA cold, not actual cold weather, what do you guys who experience "winter" think?


Is there interest in this? Wired or wireless?
----------

https://youtu.be/vH_keVQ0tiQ
```

---
## \#2 Posted by: TarzanHBK Posted at: 2016-10-06T08:32:07.112Z Reads: 295

```
first off, really cool that this works! Why not experimenting :slight_smile:
But i do have my problems with this design when it comes to safety. With just a little cramp in your hand, you´ll be fireing fullspeed in some bush or even worse, some traffic. With our current transmitter, you could just let go of the throttle and relax a bit, or if something bad happens, throw your remote away.
```

---
## \#3 Posted by: saul Posted at: 2016-10-06T08:45:43.098Z Reads: 279

```
ok so this is just a very very quick proof of concept and yea it works!
I should be more clear.

 There are two  6mm diameter **magnets** on the index finger with about **30mm** space between. 1 + and 1 - 
The hall **sensor** is on the **thumb**.

So thumb to  tip of index = **_Brake_**
thumb to index knuckle = **_Go_**

The distance from each varies just like a regular remote. and if your thumb is not near either magnet it is **neutral!** 

I can add some kind of safety switch like bb if that makes you feel better.... :upside_down:
```

---
## \#4 Posted by: TarzanHBK Posted at: 2016-10-06T08:49:10.432Z Reads: 248

```
okok interesting concept! 
yah why not :) test it a bit to avoid some starting issues with the design and i think some people would be very interested to use these when it gets colder outside now.
Of course the wireless one, noone likes cables :monkey:
```

---
## \#5 Posted by: saul Posted at: 2016-10-06T09:10:09.279Z Reads: 223

```
Cool, i'm already working with the mini remote which is small enough to stick to back of the glove, so nearly hands free.

hopefully i can swap the pot for a hall sensor with no mods...
```

---
## \#6 Posted by: scottkellum Posted at: 2016-10-06T12:41:58.496Z Reads: 191

```
Nice! I'm working on a power glove with a bend sensor in the middle finger. Nice to see your approach and interested in seeing where this goes.

Edit: some details: I'm modding a torqueboards remote with a bend sensor and 22k ohm resistor to get the right signal. I'm programming the thresholds into the VESC. Worked out to be relatively simple and straightforward, sensor just works on the remote.
```

---
## \#7 Posted by: treenutter Posted at: 2016-10-06T13:03:23.672Z Reads: 182

```
[quote="saul, post:1, topic:10718"]
what do you guys who experience "winter" think?
[/quote]


@saul I like the concept! I live in the Eastern US and it's already dropping to 40F in the mornings here. It is hard to control my standard remote with gloves on, so my controller hand is usually gloveless and it gets miserable on long rides. I'd love to see an alternative.
```

---
## \#8 Posted by: saul Posted at: 2016-10-06T17:13:22.612Z Reads: 157

```
I saw that video like a day after i ordered the sensors which were just added on to see if this would work.

I've never worked with bend sensors or even seen one lol 
but hall sensors seem to be a drop in replacement for a pot, just solid state :nerd:, 
makes sense since its all on an analog line.

so far this has been really easy too, It only took a few minute to hack this together...
```

---
## \#9 Posted by: saul Posted at: 2016-10-06T17:26:11.609Z Reads: 152

```
that is really cold! with the wind I don't know how you can ride without gloves.

I would have been on this so much faster if there was that one season here...but yea :sunglasses:
```

---
## \#10 Posted by: saul Posted at: 2016-10-06T17:30:00.318Z Reads: 155

```
literally just wired in place of ch2 pot on the mini remote and it works wireless!
just a servo on my desk but response is really good for v.001 :nerd:
```

---
## \#11 Posted by: saul Posted at: 2016-12-03T00:15:12.226Z Reads: 104

```
Its been a bit but I finally came back to this, added a custom 3d printed enclosure.

Check it out in action. Sorry for the camera angles! :grin:
https://www.youtube.com/watch?v=D-noNwGkBHQ
```

---
## \#12 Posted by: themegak Posted at: 2016-12-03T02:42:48.247Z Reads: 98

```
Wow.  That is really cool.  How much did it cost all in to make it ?  Also do you need to use a big glove or can you use any glove ?
```

---
## \#13 Posted by: saul Posted at: 2016-12-03T10:04:23.753Z Reads: 85

```
Not much just materials and time. Most gloves should work, one that fits well is best of course.

More updates coming soon.
```

---
