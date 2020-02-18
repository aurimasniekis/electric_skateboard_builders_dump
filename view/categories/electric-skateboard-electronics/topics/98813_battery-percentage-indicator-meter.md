# Battery Percentage Indicator/Meter

### Replies: 5 Views: 191

## \#1 Posted by: longboardshort Posted at: 2019-07-20T22:04:09.020Z Reads: 84

```
Hello everyone, first and foremost sorry if this has been covered elsewhere already as I imagine it was.  However I can’t find it.

So for all of my builds and it’s pretty standard that most of us use battery meters of some sort, whether it be for LiPo/Li-ion batteries. So for LiPo batts, it’s recommended to not ride below roughly 60% to play it safe, and I think a bit lower (like 50% for Li-ion).

This is to help increase the lifetime/cycle of our batteries due to lithium battery chemistry. I just build a diy board for a friend and rather than just telling them not to ride below 60% on the meter, what can be done or can someone point me in the direction of a meter that can factor in this offset? Essentially all I’m asking is if there are any existing solutions to get a battery meter that, let’s just say for LiPo for example turn the usable 40% of the battery and display that as the 0-100%?

I know this is also accounted for in the Vesc software via voltage cutoff limits, but I’m specifically looking for a display representation of what I’ve already mentioned above.

As always, any and all hell is much appreciated, and I’m sorry if this is already covered somewhere else >.< cheers everyone and stay cool out there in those scorchers! 🔥🔥
```

---
## \#2 Posted by: accrobrandon Posted at: 2019-07-21T03:37:28.490Z Reads: 72

```
Most affordable meters come pre programmed with specs... The only option I can offer u is to set the series count higher so it reads 0 sooner... So say for a 10s battery u set the meter to 12s... So what it thinks is an empty 12s value is wher youd want to stop... Best I can think without going custom... But probably more work than just checking the board every so often....
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-07-21T05:37:13.500Z Reads: 60

```
The other option is to get a volt meter and just learn what voltage equates to 60% SOC. I don't know of any percentage meters that have flexible enough adjustment for your requirements.

I suppose if you were really determined you could get a small microcontroller and a display and build a meter from scratch, but that's a lot of work.
```

---
## \#4 Posted by: longboardshort Posted at: 2019-07-22T00:30:05.749Z Reads: 41

```
Can anyone point me in the direction of doing something similar mentioned above in the responses as far as going about making a diy battery meter for this similar situation?
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-07-22T02:23:45.042Z Reads: 35

```
Parts I would probably use:
An arduino nano or other similar microcontroller
Some kind of power supply (probably a linear regulator)
a 2.5 digit 7 segment display

Hook all that together right, write some basic code, upload it, and you've got yourself a DIY voltmeter!

This is a broad-strokes list, you're well outside the "buy modules and plug them together and they just work" level of DIY. This project will require you to know or learn electronics, soldering and some mild coding, or have someone who does willing to do the work for you.
```

---
