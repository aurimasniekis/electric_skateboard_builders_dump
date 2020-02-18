# Flipsky 6.6 plus vs Flipsky 6.6

### Replies: 16 Views: 970

## \#1 Posted by: Rcsup1 Posted at: 2019-04-18T21:15:30.670Z Reads: 285

```
Hi all,

I was getting ready to pull the trigger here and wanted to know which of these was better. The 6.6 Plus seems to have an entirely different architecture the the original. 

The original seems beefier with Caps while the newer model lacks those caps and is smaller. I searched but did not find any conclusive information.  

Which one of these is holding up better in the real world?

Any know issues with one vs the other?
```

---
## \#2 Posted by: brenternet Posted at: 2019-04-18T22:03:36.562Z Reads: 278

```
Has the 6.6 plus been out long enough for anyone to draw conclusions? I've not been following too closely but I don't think it has.

Just to add here, that form factor on the dual 6.6 plus looks extremely good.
```

---
## \#3 Posted by: brenternet Posted at: 2019-04-18T22:15:51.597Z Reads: 273

```
![6%20flipsky|559x500](upload://yG11zXdNVAGQdnRLJYks78pA1zf.png) 

These are the caps now btw, they aren't manually soldered anymore. Should decrease issues.
```

---
## \#4 Posted by: Gamer43 Posted at: 2019-04-19T02:03:40.790Z Reads: 262

```
According to engineers who designed the FOCBox Unity, smd electrolytic capacitors not glued to the board will come off in a high vibration environment.

The pro switch does not have inrush current limiting, meaning it will eventually fail after a certain number of cycles. 

The smart switch might have inrush current limiting, but there's no way to tell. The smart switch is also highside instead of lowside, since they appear to use optocouplers with photovoltaic output to drive the MOSFETs.
```

---
## \#5 Posted by: briman05 Posted at: 2019-04-19T02:52:45.501Z Reads: 249

```
So your saying they will fail sooner then the regular 6.6?
```

---
## \#6 Posted by: brenternet Posted at: 2019-04-19T07:48:12.860Z Reads: 239

```
So theoretically we could glue those caps down and ditch the switch to make this a good option?
```

---
## \#7 Posted by: Schtekarsten Posted at: 2019-04-19T07:52:51.095Z Reads: 236

```
well y same with the new 4.20 plus.
and that thing uses 2 mosfets in parallel now so it is more capable.
but that switch...
```

---
## \#8 Posted by: Rcsup1 Posted at: 2019-04-22T18:27:35.776Z Reads: 214

```
I have the same question as brenternet?
```

---
## \#9 Posted by: brenternet Posted at: 2019-04-22T18:54:57.020Z Reads: 208

```
@Deodand - Let us pick your brain about a competitor product please kind sir.

Can we just hot glue these SMD caps down and make potential vibration issues go away?
```

---
## \#10 Posted by: Deodand Posted at: 2019-04-23T16:11:25.425Z Reads: 190

```
I'd definitely glue them. They should just be epoxied from the factory in my opinion. The unity has about 2.5 millifarads bulk capacitance, if the marking on the top is denoting 100 micro farad I'd say the bulk capacitance seems a bit low at 0.9 farads. This mostly becomes a problem under super high power draw around half speed... Not sure if this is the kind of thing flipsky tests since it's pretty difficult to do on the bench.

Can't comment too much on the rest of the board. I will say if you wanna support new open source software stuff get developed for the community buy your vesc from someone else.
```

---
## \#11 Posted by: brenternet Posted at: 2019-04-23T16:18:24.078Z Reads: 186

```
Thank you for taking the time to look at that Jeff.

I get what you're saying on open source development but the load is being shared here for most of us. I've personally bought a couple of unities for my "serious" builds and this 4.20 dual is aimed at a lightweight 8/10s kicker for my car boot, there's not much in it price wise for me however and this board will probably end up with another unity on it but for budget builds where every dollar matters you can see the place for a simple, inexpensive esc like this. 

If this was $20 cheaper it would be a no brainer
```

---
## \#12 Posted by: Deodand Posted at: 2019-04-23T16:52:19.158Z Reads: 175

```
It would be hypocritical of me to be mad at anyone for it. I have bought my share of knockoff stuff when money's tight (nearly always is, isn't it?)

Just figured I'd mention it since obviously some of the pricing of the unity is worked into paying me to help address hardware/software issues and add new features. Remember that's part of what your paying for and think of it as a positive thing when you buy a unity your supporting some extra dev to make cool new stuff. No worries either way 👍
```

---
## \#13 Posted by: Gamer43 Posted at: 2019-04-23T19:33:08.131Z Reads: 169

```
If you could get BLDC integrating to work without tuning (that is, out of the box, none of that detection stuff), that would be awesome :wink: .

I have the algorithm if you want it.  

[quote="Deodand, post:12, topic:91047"]
Remember that’s part of what your paying for and think of it as a positive thing when you buy a unity your supporting some extra dev to make cool new stuff.
[/quote]

That's what they say about Arduino, except STMicroelectronics's entire Nucleo Ecosystem is cheaper than that overpriced (and honestly overrated) development platform X_X.
And STM gives you like, 10x the hardware capabilities.

Can't say the same about the unity. That thing is cool and the high level of integration is extremely impressive.
```

---
## \#14 Posted by: pookybear Posted at: 2019-05-12T23:03:36.051Z Reads: 152

```
@Gamer43 

Trying to revive this.

So the best option out of the three for fvesc 6.6 is the original one w the large caps. [This](https://flipsky.net/collections/electronic-products/products/dual-fsesc6-6-based-upon-vesc6-with-aluminum-heatsink) then?
```

---
## \#15 Posted by: RedBaron Posted at: 2019-05-12T23:14:42.252Z Reads: 151

```
I've only used the fsesc 6.6 dual you reference. Never had an issue with them. I'm curious about the 6.6plus but i wish it didn't make you use the power button. Ive heard the antispark in it is trash, but that small form factor is so nice. And I'll never wait as long as it takes to buy a unity these days so flipsky it is.
```

---
## \#16 Posted by: pookybear Posted at: 2019-05-12T23:17:01.215Z Reads: 151

```
Exactly what I was thinking too. Small form factor is what kept me going back to it. But like you said, the power switch is what's holding me back from getting it. I wonder if there's a way to bypass it. Although, they emphasized in the description to NOT plug the battery in if the switch is not connected.

I'll probably end up w the big cap version.
```

---
