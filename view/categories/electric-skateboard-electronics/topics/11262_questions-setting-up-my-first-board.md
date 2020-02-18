# Questions setting up my first board

### Replies: 11 Views: 872

## \#1 Posted by: ouch_fiyah Posted at: 2016-10-17T00:49:33.553Z Reads: 99

```
Hey everyone,

I really got into reading/researching about electric skateboards over the summer. After ordering parts (which took awhile to arrive), I forgot some of the stuff I read about :(. Now that I have time, I want to start putting my board together. So I have a few questions if anyone could answer them.

Parts:
Longboard, 83mm Wheels, Caliber Trucks, TB 16/32T pulleys (which I've already attached)
Ollinboard VESC, TB 230kv motor, 2 x Turnigy 4s1p 5000mah 25c batteries, and TB Wireless Remote


1) I spent a day trying to figure it out, but I just want confirmation. I am suppose to wire my batteries in series right? That would give me 8s1p and according to the "toddy's electric skateboard calculator", I'll be getting ~23mph. If i'm suppose to wire it in parallel, please let me know!

2) I've seen an antispark loop around the forums. In which part of my setup would I attach this? And why would I like one of these on my board?

3) I also wanted to add a voltage indicator for my battery, that would just connect at both ends of the "8s battery" right?

4) Ollin Board's VESC motor connectors are all black vs TB's motor connectors (yellow, blue, black). Does it matter which plugs go where?

5) TB's 230kv motor has a flat 6 pin connector (along with 3 motor connectors), would anyone know where the 6pin connector goes? 

I think that's all I have for physically setting up the board. After that's done, I'll tackle configuring VESC (via walkthrough post) and setting up the wireless remote.


Thanks in advance!
```

---
## \#2 Posted by: Namasaki Posted at: 2016-10-17T04:03:56.386Z Reads: 79

```
[quote="ouch_fiyah, post:1, topic:11262"]
1) I spent a day trying to figure it out, but I just want confirmation. I am suppose to wire my batteries in series right? That would give me 8s1p and according to the "toddy's electric skateboard calculator", I'll be getting ~23mph. If i'm suppose to wire it in parallel, please let me know!
[/quote]

Yes, wire the batteries in series to double the voltage.
Don't put too much faith in those speed calculators. they are just a ballpark idea and not very accurate.
```

---
## \#3 Posted by: rpn314 Posted at: 2016-10-17T04:06:15.213Z Reads: 80

```
1. Yep, series. Not sure about that speed, but sounds accurate.
2. Anything anti-spark would go in-between your vesc (or any other ESC) and your batteries. They literally prevent sparks when you connect and disconnect your batteries (ie, turn your board on and off). There's a few options from anti-spark key to a solid-state soft switch type thing. Mostly comes down to preference.
3. Yes. Red to red, black to black.
4. No, but yes. Plug them in, figure out if your motor is going the direction you want it to. If so, youre set. If not, swap two of the phase wires (ones coming out of the motor going to the VESC/ESC) and you're good,
5. That's the sensor wires. It would go in the sensor port of the VESC, if you want to use them. I have the same motor and I have been quite happy without them. There's definitely benefits to using them :), but just be aware that you'll have to match up the phase wire with the corresponding sensor wire, which can get tricky.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-10-17T04:06:33.690Z Reads: 72

```
[quote="ouch_fiyah, post:1, topic:11262"]
2) I've seen an antispark loop around the forums. In which part of my setup would I attach this? And why would I like one of these on my board?
[/quote]


Either an anti-spark loop or an electronic high voltage anti-spark switch because when you connect the power wires to your Vesc, there will be a rush of current to fill the capacitors and it will cause a tremendous spark unless you have an anti-spark device.
```

---
## \#5 Posted by: Namasaki Posted at: 2016-10-17T04:10:21.059Z Reads: 68

```
[quote="ouch_fiyah, post:1, topic:11262"]
4) Ollin Board's VESC motor connectors are all black vs TB's motor connectors (yellow, blue, black). Does it matter which plugs go where?
[/quote]

If you decide to connect the sensor wires and run sensored then it does matter and you must connect each motor wire to exactly to the right esc wire or you will burn it down.

If you don't use the sensor wires, then you can connect them any way  you want and if the motor spins in reverse, just swap any 2 wires to change it.
```

---
## \#6 Posted by: rpn314 Posted at: 2016-10-17T04:13:03.702Z Reads: 61

```
Sorry for stepping on your toes @Namasaki! Didn't see your reply until I'd finished mine.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-10-17T04:16:56.724Z Reads: 56

```
No worries bro! We are reinforcing each others comments.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-10-17T04:20:46.848Z Reads: 58

```
I have never found speed calculators to be totally accurate because of factors that they don't account for.
Like rider weight, wind resistance, voltage sag, esc efficiency,
```

---
## \#9 Posted by: ouch_fiyah Posted at: 2016-10-17T13:07:19.345Z Reads: 52

```
Thanks a lot @Namasaki and @rpn314!

And the motor has 3 bullet connectors (and a 6 pin connector), I just keep switching the 3 bullet connectors until the motor spins the correct way? 

Lastly (for now), where would I wire in a power switch? 

Thanks again for the help guys. I'll update when I get more things assembled, SO EXCITED.
```

---
## \#10 Posted by: rpn314 Posted at: 2016-10-17T15:14:44.275Z Reads: 42

```
Our pleasure!

Yes. Personal recommendation is do motor detection and setup before figuring out direction.

I have mine set up Y-Blu-Blk on one vesc and Blk-Blu-Y on the other. I found that's what gave my motors the direction I needed, but it really doesn't matter. I just started somewhere and flipped a few wires (I don't actually remember where I started) until they were both spinning the right way.

If you want to set up the hall sensors, just let us know. It's a little more than just plug it in until it works. You have to match the main phase wires with their corresponding sensor wires. But that's only if you want to do that. It's not necessary with the VESC.

If you were to wire in a power switch (either a loop key or a anti-spark switch like what TB and others sell, or that you can make yourself if you want), it would be between the battery and the vesc.

Good tag team then @Namasaki :punch: (closest thing to a fist bump I could find)
```

---
## \#11 Posted by: Namasaki Posted at: 2016-10-17T15:42:39.792Z Reads: 38

```
Right on bro! 👊
```

---
